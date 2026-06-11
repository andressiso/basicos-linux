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
· ssh-keygen -t ed25519 -C andres.siso.lopez@gmail.com

Iniciar el agente SSH:
· eval "$(ssh-agent -s)"

Añadir la clave:
· ssh-add ~/.ssh/id_ed25519

Mostrar la clave pública:
· cat ~/.ssh/id_ed25519.pub

La clave privada se almacena en ~/.ssh

## Comandos Git
git status

git remote -v

git add .

git commit -m "Comentario"

git push

