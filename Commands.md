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

>git commit -m "mensaje descriptivo"

Confirma los cambios de los archivos que se encuentran en el stage y genera un registro en el historico de cambios (log). Recuer que un commit es un hito en el tiempo.

>git commit --amend -m "mensaje descriptivo"

Permite modificar el mensaje de un commit local que aun no ha sido publicado (git push). Tambien permite agregar cambios al ultimo commit. Agrega o modifica archivos y ejecuta el comando nuevamente.

>git diff | git diff nombre-archivo | git diff ruta-archivo

Este comando permite ver las diferencias entre el archivo actual (aquel que sufrió cambios) y la versión de este mismo archivo que se guardo en el ultimo commit.

>git checkout .

Permite revertir todos los cambios no guardados en el stage, es decir regresa el codigo fuente al ultimo commit.
Revierte cambios guardados con Control + S

>git checkout nombre-archivo.extension | git checkout ruta-archivo.extension | git checkout .extension | git checkout carpeta/ | git checkout carpeta/*.extension

Revierte el o los archivos a la version del ultimo commit.
Revierte cambios guardados con Control + S

>git log | git log --oneline

Permite obtener el historico de los commits realizados. La variante --oneline muestra el historico de commits en una sola linea.

