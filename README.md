# git-github-notes
Notas de GitHub
[Curso Profesional de Git y GitHub en Platzi](https://platzi.com/clases/git-github/)


| Comando | Descripción |
|---------|-------------|
|`git init`|Crear nuevo repositorio local.|
|`git add <file>`|Agregar archivo al stage.|
|`git add .`|Agregar todos los archivo con cambios al stage.|
|`git rm --cached <file>`|Elimina los archivos del área de Staging y del próximo commit pero los mantiene en nuestro disco duro.|
|`git rm --force <file>`|Elimina los archivos de Git y del disco duro. Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podremos recuperarlos si es necesario (pero debemos usar comandos más avanzados).|
|`git branch`|Listar todas las ramas.|
|`git switch <branch>`|Cambiar de rama existente.|
|`git status`|Estado del repo.|
|`git commit -m "mensaje"`|Agregar commit al repositorio.|
|`git push origin <branch>`|Enviar los cambios al repo remoto.|
|`git config`|Ver todas las configuraciones.|
|`git config --list`|Ver todas las configuraciones por defecto.|
|`git config --list --show-origin`|Ver ubicación de las configuraciones.|
|`git config --global user.email "tu@email.com"`|Configurar tu email.|
|`git config --global user.name "Tu Nombre"`|Configurar tu nombre.|
|`git remote add origin <REPO-URL>`|Clonar y traer un repo remoto.|
|`git remote -v`||
|`git pull origin master`|Descargar los cambios desde el repositorio remoto.|
|`git show <file>`|Mostrar los cambios sobre un archivo.|
|`git diff`|Ver todos los cambios.|
|`git diff <commit1> <commit2>`|Ver diferencias entre commits.|
|`git log`|Ver todos los cambios.|
|`git log --stat`|Ver cambios detallados.|
|`git reset --soft`|Borramos todo el historial y los registros de Git pero guardamos los cambios que tengamos en Staging, así podemos aplicar las últimas actualizaciones a un nuevo commit.|
|`git reset --hard`|Borra todo. Todo todito, absolutamente todo. Toda la información de los commits y del área de staging se borra del historial.|
|`git reset HEAD`|Retirar todos los archivos del staging, sin borrarlos.|
|`git checkout <commit> <file>`|Obtener versión del archivo.|
|`git checkout master <file>`|Obtener versión del archivo que está en master.|
|||
|||
|||
|||
|||
|||