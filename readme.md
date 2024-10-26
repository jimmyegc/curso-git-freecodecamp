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

-git checkout <commit> : Para verificar el código que hay en ese commit.

-git revert HEAD : quitar los cambios que ya se añadieron al commit.
-git rever HEAD --no-edit

-git commit --amend -m "feat: my complete change" : sí olvidaste un cambio lo agrega al último commit.

Ramas:

-git checkout -b develop : Crea y cambia a la rama develop
-git branch : listar las ramas
-git checkout main : cambiar a la rama main