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

>git log | git log --oneline | git log --oneline -n

Permite obtener el historico de los commits realizados. La variante --oneline muestra el historico de commits en una sola linea y la variante -n indica la cantidad de commits a visualizar.

>git reset | git reset nombre-archivo.extension | git reset .extension | git reset nombre-carpeta | git reset nombre-carpeta/.extension

Remueve el o los archivos contenidos en la zona stage, mas no elimina los cambios realizados en el o los archivos.
Remueve git add

>git reset commit-id | git reset --mixed commit-id

Retorna el codigo a un commit en especifico y mantien los cambios, retira los archivos modificados de la zona del stage.

>git reset --soft HEAD~1 | git reset --soft commit-id

Remueve el ultimo commit, pero mantiene los cambios de los archivos modificados. La variante commit-id se ubica en el commit indicado y mantiene los cambios.

>git reset --hard HEAD~1 | git reset --hard commit-id

Remueve el ultimo commit, y borra los cambios de los archivos modificados. La variante commit-id se ubica en el commit indicado y elimina los cambios en los archivos.

>git help comando-ayuda

Muestra las posibles variantes del comando indicado.

> git revert HEAD | git revert commit-a-eliminar

Este comando permite deshacer un commit ya publicado (git push). Para esto crea un commit que elimina los cambios indicados en el commit a eliminar (HEAD o commit-a-eliminar).

>git config --global alias.<letra> "<comando>" 

Permite utilizar un comando a través de la asignación de un alias. Donde comando es por ejemplo, status, log u otro y letra es s, l o cualquiera que desee asignar. 

>git config --get-regexp alias

Lista los alias creados en Git

>git config --global --unset alias.tu-alias

Con el comando anteior se puede eliminar un alias, para esto se debe reemplazar tu-alias con el valor que hayas asignado al alias que desees eliminar.

>git mv nombre-archivo.extension nuevo-nombre-archivo.extension

El comando permite cambiar el nombre de un archivo, luego de esto git seguira en supervision del control de versiones.

>git rm nombre-archivo.extension

Elimina o remueve un archivo y permite que esta accion se vea reflejada en el historico de cambios.

>git reflog

Lista el historico de cambios y acciones realizadas.

>Creacion del archivo .gitignore

Este archivo deb ubicarse al nivel de la carpte .git. Su contnido debe tener los siguiente y depende de lo que desees ignorar.

- Carpeta: /nombre-carpeta/
- Carpeta y un archivo: /nombre-carpeta/nombre-archivo.extension
- Carpeta y varios archivos: /nombre-carpeta/**.extension
- Archivo: nombre-archivo.extension
- Archivos con la misma extension: **.extesion

[View gitignore generator online](https://www.toptal.com/developers/gitignore)
[View gitignore template files](https://github.com/github/gitignore)