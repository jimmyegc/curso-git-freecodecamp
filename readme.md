# Curso de Git desde Cero - Aprende Git
[Curso de Git desde Cero - Aprende Git](https://www.youtube.com/watch?v=h2ZzlNVl-nI)

## Estados

Preparado o Stage: Modificación y agregamos para su confirmación.
- Modificado: Archivos que hemos modificado de su anterior version.
- Confirmado: Snapshot / updated.
- U: Untrack, no tiene seguimiento del archivo y sus cambios.

- git restore index.html -- quita el archivo del workdirectory.
- git commit -m "feature: xxx"
- git status

- git log 
- git log --oneline

- git checkout <commit> : Para verificar el código que hay en ese commit.

- git revert HEAD : quitar los cambios que ya se añadieron al commit.
- git rever HEAD --no-edit

- git commit --amend -m "feat: my complete change" : sí olvidaste un cambio lo agrega al último commit.

## Ramas

- git checkout -b develop : Crea y cambia a la rama develop
- git branch : listar las ramas
- git checkout main : cambiar a la rama main
- git branch -d feature/my-new-feature: para eliminar una rama.

## Stashs

- git stash : guardar en una pila temporal para movernos entre las ramas.
- git stash -u : para guardar la pila y añadir los elementos nuevos a ese stash.
- git stash pop: para sacar el elemento de la pila.
- git stash list : Listar todos los stashs.
- git stash apply : Regresa el stash pero sin sacarlos de la lista.
- git stash pop stash@{0} : Sacando el stash especifico.
- git stash branch feature/my-stashed-feature stash@{0} : Hace una rama a partir de un Stash.
- git stash drop stash@{0} : Elimina el stash necesario.
- git stash clear : limpiar todos los stash.

## Cherry Pick
Escenario: Hacemos una modificación en develop que es parte de un cambio que voy a trabajar.

- Se toma el hash del commit: develop/ec381a0 
- Irse a la rama destino: git checkout feature/my-new-feature
- git cherry-pick ec381a0 

## Merge
Mezclamos la rama new feature con develop para test.

- Revisamos que todo este añadido en la rama: feature/my-new-feature
- Nos cambiamos a develop
- git merge feature/my-new-feature : colocamos la rama que queremos mezclar

## Conflictos

- git checkout -b feature/my-awesome-feature : Se hace una nueva rama en develop.
- Otro colega hace un cambio en develop: (mientras yo estoy en mi rama).
- Termino mi cambio en mi rama, hago el commit del feature.
- git merge feature/my-awesome-feature : Hago el merge de mi rama con feature y resuelvo los conflictos.
- Resolver conflictos...
- git add .
- git commit -m "feat: conflict solution"

## Customizar Git Bash
[Customize Bash](https://youtu.be/Bkaox81ppds?si=YHl4Njtb3iU5gOQt)
