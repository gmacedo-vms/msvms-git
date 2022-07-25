## Git Log

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

> git log --graph --pretty=oneline

> git log --graph --oneline

> git log --all --decorate --oneline --graph

> git log --all --graph --since=2022-01-01 --oneline

> git log --all --graph --since=2022-01-01

> git log --abbrev-commit | git log --abbrev-commit --oneline

> git log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all

> git log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)' --all

[View Command Init](Init.md)

[View Command Merge](Merge.md)

[View Commands](../Commands.md)