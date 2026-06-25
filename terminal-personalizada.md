Personalizando mi terminal en Fedora (sin perder de vista lo importante)

Hoy he dedicado un rato a dejar mi entorno de terminal en Fedora más cómodo para trabajar. No buscaba una terminal espectacular visualmente, sino un entorno limpio y que me ayude a aprender Linux.

Punto de partida

Mi configuración actual es:

Fedora KDE
Konsole
Zsh
Oh My Zsh

Inicialmente utilizaba Powerlevel10k, un tema muy popular para Zsh. Después de probarlo durante un tiempo decidí eliminarlo.

El motivo no fue que funcionase mal, sino que prefería un prompt mucho más sencillo, con un formato clásico:

andres@fedora:~/ruta$

Para aprender Linux, creo que un prompt simple resulta más cómodo y distrae menos que uno lleno de información adicional.

Plugins que sí he decidido mantener

He instalado tres herramientas que considero realmente útiles porque no sustituyen los comandos tradicionales.

zsh-autosuggestions

Sugiere comandos basándose en el historial mientras escribes.

No ejecuta nada automáticamente ni cambia mi forma de trabajar; simplemente me recuerda comandos que ya he utilizado anteriormente.

zsh-syntax-highlighting

Resalta los comandos mientras los escribo.

Si un comando existe, aparece con un color diferente al de uno inexistente. Es una ayuda sencilla para detectar errores antes de pulsar Enter.

fzf

Permite buscar rápidamente en el historial y en otros listados de forma interactiva.

De momento apenas lo estoy utilizando porque quiero acostumbrarme primero al funcionamiento normal del historial de Zsh, pero me parece una herramienta interesante para el futuro.

Decisiones que he tomado

He decidido no utilizar:

alias personalizados
reemplazos de comandos (eza, bat, etc.)
prompts muy recargados
iconos en la terminal

Prefiero aprender utilizando las herramientas estándar (ls, cat, grep, find...) antes de añadir capas de personalización.

Creo que, a largo plazo, esto hará que me sienta cómodo utilizando prácticamente cualquier sistema Linux, incluso aquellos que no tengan mi configuración personal.

Próximo objetivo

Ahora que la terminal está lista, el siguiente paso será configurar el entorno de juegos en Fedora utilizando una biblioteca de Steam sobre una partición ext4 para evitar los problemas que encontré al intentar ejecutar juegos con Proton desde una partición NTFS.
