## Git Checkout 

> git checkout .

Permite revertir todos los cambios no guardados en el stage, es decir regresa el codigo fuente al ultimo commit.
Revierte cambios guardados con Control + S

> git checkout nombre-archivo.extension | git checkout ruta-archivo.extension | git checkout .extension | git checkout carpeta/ | git checkout carpeta/*.extension

Revierte el o los archivos a la version del ultimo commit.
Revierte cambios guardados con Control + S

> git checkout nombre-rama

Permite ubicarse a la rama que se indique.

> git checkout -b nombre-rama

Crea una rama y se ubica en la rama creada.

> git checkout [commit] -- [archivo]

Retorna un archivo especifico al commit indicado.

[View Command Branch](Branch.md)

[View Command CherryPick](CherryPick.md)

[View Commands](../Commands.md)