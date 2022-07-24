##Git Log

> git log | git log --oneline | git log --oneline -n | git log --oneline --decorate --all --graph

Permite obtener el historico de los commits realizados. La variante --oneline muestra el historico de commits en una sola linea y la variante -n indica la cantidad de commits a visualizar.

> git log origin/nombre-rama..HEAD

Ver los commits pendiente de subir al repositorio de github en la rama indicada (nombre-rama).

> git log --follow -p [filename]

Mustra los cambios realizados en los commits en donde se modifico un determinado archivo.

> git log --follow --oneline [filename]

Mustra los commits en donde se modifico un determinado archivo.

> git log --all --grep='palabra-clave'

Muestro los commits que tienen como mensaje la palabra clave.

> git log --pretty=oneline

> git log --stat

> git log --graph

> git log --abbrev-commit | git log --abbrev-commit --oneline

[View Command Init](Init.md)

[View Command Merge](Merge.md)

[View Commands](../Commands.md)