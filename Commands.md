#Commands

>git init 

Inicializa la carpeta actual como un repositorio. Se crea la carpeta **.git**

>git status

Muestra las carpetas/archivos a los cuales git realiza o no el control de versiones. Los siguientes colores indican lo siguiente.
- Rojo: Son archivos nuevos o modificados, a los nuevos Git no realiza control de veriones.
- Verde: Archivo que se encuentran en el stage pendientes de una confirmacion (commit).

> git add . | git add -A | git add --all

Git inicia el control de versiones a todos los archivos nuevos o modificados los cuales no estaban siendo controlados y los aniade a la zona del stage.

> git add nombre-archivo.extension | git add ruta-archivo.extension | git add .extension | git add carpeta/ | git add carpeta/*.extension

Git agrega al stage el archivo o carpeta indicado e inicia el control de versiones sobre el mismo.


