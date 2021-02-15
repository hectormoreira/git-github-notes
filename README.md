# git-github-notes
> Notas de GitHub [Curso Profesional de Git y GitHub en Platzi](https://platzi.com/clases/git-github/)


| Comando | Descripción |
|---------|-------------|
|`git init`|Crear nuevo repositorio local.|
|`git add <file>`|Agregar archivo al stage.|
|`git add .`|Agregar todos los archivo con cambios al stage.|
|`git rm --cached <file>`|Elimina los archivos del área de Staging y del próximo commit pero los mantiene en nuestro disco duro.|
|`git rm --force <file>`|Elimina los archivos de Git y del disco duro. Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podremos recuperarlos si es necesario (pero debemos usar comandos más avanzados).|
|`git status`|Estado del repo.|
|`git commit -m "mensaje"`|Agregar commit al repositorio.|
|`git config`|Ver todas las configuraciones.|
|`git config --list`|Ver todas las configuraciones por defecto.|
|`git config --list --show-origin`|Ver ubicación de las configuraciones.|
|`git config --global user.email "tu@email.com"`|Configurar tu email.|
|`git config --global user.name "Tu Nombre"`|Configurar tu nombre.|
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
|Repositorios Remotos|----------------|
|`git remote add origin <REPO-URL>`|Clonar y traer un repo remoto.|
|`git remote -v`|Ver orígenes|
|`git pull origin master`|Descargar los cambios desde el repositorio remoto.|
|`git branch <name_branch>`|Crear nueva rama.|
|`git branch`|Listar todas las ramas.|
|`git show-branch`|Listar todas las ramas e historia.|
|`git show-branch --all`|Listar todas las ramas e historia.|
|`git checkout <branch>`|Moverse entre ramas.|
|`git merge <branch>`|Hacer merge entre ramas.|
|`gitk`|Ver historial visual de git|
|`git push origin master`|Enviar los cambios al repo remoto master.|
|`git merge <branch>`|Fusionar ramas|
|Configurar llaves|----------------|
|`ssh-keygen -t rsa -b 4096 -C "tu_email@dominio.com"`|Generar llave. -t = Especifica cual es el algoritmo que vamos a usar para crear esa llave. rsa = Algoritmo a usar, hasta el momento el mas popular. -b = Especifica que tan compleja es la llave. 4096 = Complejidad de la llave desde una perspectiva matemática. -C = Indica a que correo electrónico va estar conectado esta llave|
|`eval $(ssh-agent -s)`|Evaluar servidor ssh activo|
|`ssh-add ~/.ssh/id_rsa`|Agregar llave privada|
|`alias <nombre_alias> "<comando>"`|Crear nuevos alias|
|`git tag -a v0.1 -m "mensaje" <hash_commit>`|Crear tags, los tags pueden usarse como releases|
|`git tag`|Ver todos los tags|
|`git show-ref --tags`|Ver todos los tags con referencias|
|`git push origin --tags`|Enviar tags a github|
|`git tag -d <nombre_tag>`|Eliminar tag|
|`git push oprigin :refs/tags/<nombre_tag> `|Eliminar la referencia del tag en github|
|||
|||
|||
|||