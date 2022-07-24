##Git Config

> git config --global alias.<letra> "<comando>"

Permite utilizar un comando a través de la asignación de un alias. Donde comando es por ejemplo, status, log u otro y letra es s, l o cualquiera que desee asignar.

> git config --get-regexp alias

Lista los alias creados en Git

> git config --global --unset alias.tu-alias

Con el comando anteior se puede eliminar un alias, para esto se debe reemplazar tu-alias con el valor que hayas asignado al alias que desees eliminar.

[View Command Commit](Commit.md)

[View Command Diff](Diff.md)

[View Commands](../Commands.md)