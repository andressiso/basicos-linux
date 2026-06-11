# GIT y GITHUB
Git trabaja localmente
GitHub es una plataforma

Los cambios no aparecen en GitHub hasta realizar:
1. Commit
2. Push

Borrar un archivo localmente no lo elimina automáticamente del repositorio remoto.

## Autenticacion en GitHub

Al ejecutar:
git push -u origin main

GitHub devolvía :
"Password authentication is not supported for Git operations."

GitHub ya no permite autenticarse mediante contraseña para operaciones Git.
En la plataforma tuve que activar la autenticacion por SSH.

## SSH
SSH utiliza un par de claves:
·Clave privada: permanece en mi equipo.
·Clave pública: se comparte con el servicio remoto.

Primero hay que generar la clave :

ssh-keygen -t ed25519 -C andres.siso.lopez@gmail.com

Iniciar el agente SSH:

eval "$(ssh-agent -s)"

Añadir la clave:

ssh-add ~/.ssh/id_ed25519

Mostrar la clave pública:

cat ~/.ssh/id_ed25519.pub

La clave privada se almacena en ~/.ssh

## Comandos Git
git status -> Comando fundamental para comprobar el estado del repositorio. Utilizar antes de hacer commit o push cuando no funcione.

git add . -> Prepara los cambios

git commit -m "Comentario" -> Crea un punto en el historial local

git push -> Envía los commits a GitHub

## Remoto del Repositorio

Comprobar remoto:

git remote -v


Cambiar de HTTPS a SSH:
git remote set-url git@github.com.com:usuario/repositorio.git 
