# Configuracion global
git config --global user.name | user.email

# Agregar al staging un archivo
git add archivo.txt

# Agregar al staging todo lo que este en working area
git add .

# Hacer un commit
git commit -m "agrega un commit"

# Agregar al staging y hace el commit (funciona con archivos ya existentes)
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


