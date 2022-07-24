## Git Reset 

> git reset | git reset nombre-archivo.extension | git reset .extension | git reset nombre-carpeta | git reset nombre-carpeta/.extension

Remueve el o los archivos contenidos en la zona stage, mas no elimina los cambios realizados en el o los archivos.
Remueve git add

> git reset commit-id | git reset --mixed commit-id

Retorna el codigo a un commit en especifico y mantien los cambios, retira los archivos modificados de la zona del stage.

> git reset --soft HEAD~1 | git reset --soft commit-id

Remueve el ultimo commit, pero mantiene los cambios de los archivos modificados. La variante commit-id se ubica en el commit indicado y mantiene los cambios.

> git reset --hard HEAD~1 | git reset --hard commit-id

Remueve el ultimo commit, y borra los cambios de los archivos modificados. La variante commit-id se ubica en el commit indicado y elimina los cambios en los archivos.

[View Command Remote](Remote.md)

[View Command Restore](Restore.md)

[View Commands](../Commands.md)