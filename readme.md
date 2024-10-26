# Curso de Git desde Cero - Aprende Git
https://www.youtube.com/watch?v=h2ZzlNVl-nI


Notas:

Estados:

-Preparado o Stage: Modificación y agregamos para su confirmación.
-Modificado: Archivos que hemos modificado de su anterior version.
-Confirmado: Snapshot / updated.

- U : Untrack, no tiene seguimiento del archivo y sus cambios.

-git restore index.html -- quita el archivo del workdirectory.
-git commit -m "feature: xxx"
-git status

-git log 
-git log --oneline
-git log --oneline main

-git checkout <commit> : Para verificar el código que hay en ese commit.

Tags:
-git checkout v1 : create tag "v1"
-git tag -d v1 : delete tag "v1"

git restore --staged readme.md : Deshacemos el cambio que agregamos a staged, no perdemos el cambio del archivo sólo no lo agregamos.
