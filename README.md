# git-github-notes
> Notas de GitHub [Curso Profesional de Git y GitHub en Platzi](https://platzi.com/clases/git-github/)


| Comando | Descripción |
|---------|-------------|
|`git init`|Crear nuevo repositorio local.|
|`git add <file>`|Agregar archivo al stage.|
|`git add .`|Agregar todos los archivo con cambios al stage.|
|`git rm --cached <file>`|Elimina los archivos del área de Staging y del próximo commit pero los mantiene en nuestro disco duro.|
|`git rm --force <file>`|Elimina los archivos de Git y del disco duro. Git siempre guarda todo, por lo que podemos acceder al registro de la existencia de los archivos, de modo que podremos recuperarlos si es necesario (pero debemos usar comandos más avanzados).|
|`rm -rf .git*`|Remover todas las referencias a git|
|`git rm -rf .git*`|Remover archivos de rastreo de git, sirve para nuevo clone.|
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
|`git reflog`|Ver listado de HEAD y commits, historial.|
|`git reset --soft`|Borramos todo el historial y los registros de Git pero guardamos los cambios que tengamos en Staging, así podemos aplicar las últimas actualizaciones a un nuevo commit.|
|`git reset --hard <id_head_reflog>`|Borra todo. Todo todito, absolutamente todo. Toda la información de los commits y del área de staging se borra del historial.|
|`git reset HEAD`|Retirar todos los archivos del staging, sin borrarlos.|
|`git checkout <commit> <file>`|Obtener versión del archivo.|
|`git checkout master <file>`|Obtener versión del archivo que está en master.|
|Repositorios Remotos|----------------|
|`git remote add origin <REPO-URL>`|Traer datos de un repo remoto a mi repo local.|
|`git remote -v`|Ver orígenes del repo|
|`git remote add upstream <url_repo>`|Crea nueva fuente para traer datos|
|`git pull upstream`|Todos los cambios de upstream a nuestra rama, esto se usa cuando se trabaja con fork.|
|`git pull origin master`|Descargar los cambios desde el repositorio remoto.|
|`git branch <name_branch>`|Crear nueva rama.|
|`git branch`|Listar todas las ramas.|
|`git branch -r`|Listar todas las ramas en remoto.|
|`git branch -a`|Listar todas las ramas en remoto y local.|
|`git show-branch`|Listar todas las ramas e historia.|
|`git show-branch --all`|Listar todas las ramas e historia.|
|`git checkout <branch>`|Moverse entre ramas.|
|`git merge <branch>`|Hacer merge (fusionar) entre ramas.|
|`gitk`|Ver historial visual de git.|
|`git push origin master`|Enviar los cambios al repo remoto master.|
|`git merge <branch>`|Fusionar ramas.|
|`ssh-keygen -t rsa -b 4096 -C "tu_email@dominio.com"`|Generar llave. -t = Especifica cual es el algoritmo que vamos a usar para crear esa llave. rsa = Algoritmo a usar, hasta el momento el mas popular. -b = Especifica que tan compleja es la llave. 4096 = Complejidad de la llave desde una perspectiva matemática. -C = Indica a que correo electrónico va estar conectado esta llave.|
|`eval $(ssh-agent -s)`|Evaluar servidor ssh activo.|
|`ssh-add ~/.ssh/id_rsa`|Agregar llave privada.|
|`alias <nombre_alias> "<comando>"`|Crear nuevos alias.|
|`git tag -a v0.1 -m "mensaje" <hash_commit>`|Crear tags, los tags pueden usarse como releases.|
|`git tag`|Ver todos los tags.|
|`git show-ref --tags`|Ver todos los tags con referencias.|
|`git push origin --tags`|Enviar tags a github.|
|`git tag -d <nombre_tag>`|Eliminar tag.|
|`git push origin :refs/tags/<nombre_tag> `|Eliminar la referencia del tag en github.|
|`git clone <url_repo>`|Clonar repositorio.|
|`git rebase <branch>`|Reorganiza el trabajo realizado. rebase reescribe la historia del repositorio, cambia la historia de donde comenzó la rama y **solo debe ser usado de manera local./**|
|`git stash`|Guardar cambios en memoria y recuperarlos después|
|`git stash list`|Ver lista de stash|
|`git stash pop`|Recuperar los últimos cambios desde el stash a tu staging area.|
|`git stash apply stash@{<num_stash>}`|Retomar los cambios de un stash.|
|`git stash branch <nombre_de_la_rama>`|Crear una rama con el stash.|
|`git stash branch nombre_de_rama stash@{<num_stash>}`|Crear una rama y aplicar un stash específico (obtenido desde git stash list)|
|`git stash drop`|Borrar stash.|
|`git clean --dry-run`|Simular lo que se borrará.|
|`git clean -f`|Borrar archivos no traqueados.|
|`git commit --amend`|Añade archivos y cambia mensaje en el último commit.|
|`git grep <palabra>`|Buscar palabras usadas en el repositorio.|
|`git grep -n <palabra>`|Buscar palabras usadas en el repositorio + linea.|
|`git grep -c <palabra>`|Buscar palabras usadas en el repositorio + cantidad.|
|`git log -S "palabra"`|Buscar las veces que se usó una palabra en los commits.|
|`git shortlog -sn`|Log por persona de los cambios.|
|`git shortlog -sn --all`|Todos los cambios por personas.|
|`git shortlog -sn --all --no-merges`|Todos los cambios por personas sin merges.|
|`git config --global alias.stats "shortlog -sn --all --no-merges"`|Crear un alias global|
|`git blame <archivo> -c`|Ver cambios del archivo con usuario.|
|||
|||