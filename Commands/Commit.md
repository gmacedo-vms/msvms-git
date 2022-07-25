## Git Commit

> git commit -m "mensaje descriptivo"

Confirma los cambios de los archivos que se encuentran en el stage y genera un registro en el historico de cambios (log). Recuer que un commit es un hito en el tiempo.

> git commit -am "mensaje descriptivo"

Agregar los cambios de los archivos modificados al Stage (no archivos nuevos) y genera un registro en el historico de cambios

> git commit --amend -m "mensaje descriptivo"

Permite modificar el mensaje de un commit local que aun no ha sido publicado (git push). Tambien permite agregar cambios al ultimo commit. Agrega o modifica archivos y ejecuta el comando nuevamente.

> git commit --amend --no-edit

Añade más archivos al último commit sin escribir o editar el mensaje del commit.

[View Command Clone](Clone.md)

[View Command Config](Config.md)

[View Commands](../Commands.md)
