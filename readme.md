# Configuracion global
git config --global user.name | user.email

# Agregar al staging un archivo
git add archivo.txt

# Agregar al staging todo lo que este en working area
git add .

# Hacer un commit
git commit -m "agrega un commit"

# Agregar al staging y hacer commit (aplica solo para modificaciones, no nuevos archivos)
git commit -am "un add y un commit al mismo tiempo"

# Cambiar entre commits
git checkout hash

# Regresar al commit mas actual
git checkout branchName | .

# Borrar último commit del versionado, baja los cambios al working area
git reset HEAD-1

# Borrar último commit definitivamente
git reset --hard HEAD~1
Nota: ~1 indica que se borra 1, 2 o mas commits

# revert, actualiza el head con un commit anterior, 
# lo coloca como mas rciente, mantiene pero mantiene el historial
git revert HEAD

# crear rama
git branch branchName

# listar ramas
git branch

# cambiar de rama
git checkout branchName

# crear nueva rama y cambiarse a ella
git checkout -B branchName

# realizar merge
git checkout currentBranch
git merge branchNameOrigin

# agregar un repositorio remoto
git remote add origin myUrl

# cambiar repositorio remoto
git remote set-url origin myNewUrl

# subir una rama
git push remoteAliasName remoteBranchName

# subir todas las ramas desde el local al remoto
git push --all origin

# subir cambios a una rama
git push origin branchName

# clonar un repo
git clone mySshUrl | myHttpsUrl

# crear un tag en el commit actual
git tag 0.0.1

# crear un tag de un commit especifico
git tag -a 0.0.0 myHash -m "tag 0"

# ver mis tags
git tag --list

# subir tags 
git push --tags

# eliminar un tag local
git tag -d myTag

# eliminar un tag remoto
git push origin :refs/tags/12345

# stash, pausar el trabajo y mover al "stack stash"
git stash 

# reaplicar cambios stasheados (stash mas reciente)
git stash pop

# ver pila del stash
git stash list

# reaplicar un stash espcifico
git stash apply stash@{1}

