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

# Borrar commit
git reset --hard HEAD-1
Nota: -1 indica que se borra 1, 2 o mas commits

# Borrar cambio del versionado, baja al working area
git reset HEAD-1