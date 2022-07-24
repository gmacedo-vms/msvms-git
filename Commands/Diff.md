## Git Diff

> git diff | git diff nombre-archivo | git diff ruta-archivo

Este comando permite ver las diferencias entre el archivo actual (aquel que sufrió cambios) y la versión de este mismo archivo que se guardo en el ultimo commit.

> git diff ...origin

Muestra la diferencia entre los archivos locales y los archivos ubicados en el repositorio de github.

> git diff [commit]^.. | git diff [commit]

Mustra los cambios realizados entre todos los archvos de la version actual y el commit indicado.

> git diff [commit-id]^.. --name-status

Muestra los archivos modificados entre la version actual y el commit indicado.

[View Command Config](Config.md)

[View Command Fetch](Fetch.md)

[View Commands](../Commands.md)