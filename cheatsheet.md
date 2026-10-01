# Cheatsheet de terminal y Git

pwd
* muestra en que carpeta estas

ls
* muestra lo que hay en lacarpeta

ls -la
* muestra tambien archivos ocultos como .git

cd carpeta
* entras a una carpeta

cd ..
* subes un nivel

cd ~
* regresa a tu carpeta persnal

mkdir -p a/b/c
* crea carpetas, aunque esten anidadas

rm -r carpeta
* borra una carpeta y todo su contenido

clear
* limpia la pantalla

git --version
* confirma que Git esta instalado

git config --global --list
* muestra tu nombre, correo y rama por defecto

git init
* conviete una carpeta en repositorio local

git clone url
* descarga un repo de GitHub ya conectado

git status
* muestra que cambio y que esta listo para commit

git add archivo
* prepara ese archivo para el siguiente commit

git add .
* prepara todos los cambios de la carpeta

git commit -m "mensaje"
* guarda lo preparado en el historial

git push
* sube tus commits a GitHub

git pull
* baja los cambios del equipo, hacerlo antes de trabajar

git pull --no-edit
* igual que pull pero sin abrir editor, util si el push fue rechazado

git log --oneline
* historial resumido, un commit por linea

git log --oneline -3
* verificar que se posteo en Github Si ves origin/main junto a tu commit, ya esta en GitHub

git show
* muestra el detalle del ultimo commit

git diff
* muestra lo que cambiaste despues del add

git diff --staged
* muestra lo que entraria si haces commit ahora

git restore archivo
* regresa el archivo al ultimo commit, el cambio se pierde. Tambien recupera archivos borrados

git restore --staged archivo
* saca el archivo de lo preparado, el cambio se conserva

git commit --amend -m "mensaje"
* corrige el mensaje del ultimo commit, solo si no has hecho push

git checkout -- archivo
* version pasada de git restore
