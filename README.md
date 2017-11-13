# practica13-11

Comandos de git

mkdir practica13-11
cd practica13-11
git config --global user.name "mangorex" # CONFIGURAR NOMBRE USUARIO
git config --global.user.email manuel.pc23@gmail.com # CONFIGURAR CORREO
echo "# practica13-11">> README.md
gedit README.md # ABRIR CON GEDIT Y METER MAS TEXTO
git init
git commit -a -m "first commit" # HACER COMMIT CON MENSAJE

# AÑADIMOS A NUESTRO REPOSITORIO
git remote add origin https://github.com/mangorex/practica13-11.git
git push -u origin master # HACEMOS PUSH CON NUESTRO REPOSITORIO

# PARA IGNOREAR FICHEROS HAY QUE CREAR Fichero .gitignore y escribir esos ficheros
git add .gitignore
git commit -m "Añadido git ignore"

git init
git add
git status
git commit
git commit -a -m "Cambios en README y en .gitignore" # HACER COMMIT SIN NECESIDAD DE add y con mensaje
git log
git log --oneline # MIRAR EL LOG EN UNA LINEA
git annotate <file>
git show <commit>
git checkout -b <branchName>
git branch
git status # DEBE DECIRNOS QUE VAMOS A BORRAR EL FICHERO y darnos opciones para registrar el borrado con add y demá
git checkout <branchName>
git rm fichero-a-eliminar # BORRAR ARCHIVO
git mv README leeme # RENOMBRAR ARCHIVO. No olvidarse hacer el add, el commit y el push luego
# ANTES DEL COMMIT
git reset --hard # Hacer un reset a todo antes de hacer commit, desde el último commit hecho
git checkout --filename # Hacer un reset a un fichero concreto antes de hacer commit, desde el último commit hecho

# DESPUES DEL COMMIT. ANTES DEL PUSH
git reset HEAD^ # Elimina el último commit
git commit --amend # Rectifica el último commit

git rebase -i # Añadir e
