# Configuracion global
git config --global user.name | user.email

# Agregar al staging
git add *.txt

# Hacer un commit
git commit -m "agrega un commit"

# Agregar al staging y hacer commit
git commit -am "un add y un commit al mismo tiempo"

# Cambiar entre commits
git checkout hash

# Regresar al commit mas actual
git checkout branchName | .

# Borrar commit definitivamente
git reset --hard HEAD-1
Nota: -1 indica que se borra 1, 2 o mas commits

# Borrar cambio del versionado, bajar los cambios al working area
git reset HEAD-1

# revert, actualiza el head con un commit anterior, 
# lo coloca como mas rciente, mantiene pero mantiene el historial
git revert head

# ver mi rama
git branch

# crear rama
git branch branchName

# cambiar de rama
git checkout branchName

# crear nueva rama y cambiarse a ella
git checkout -B branchName

# realizar merge
git merge branchNameOrigin

# agregar un repositorio remoto
git remote add origin myUrl

# subir todas las ramas desde el local al remoto
git push --all origin

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

# eliminar un tag
git tag -d myTag

