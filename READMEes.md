Comandos Git
============

## Versiones Traducidas
- [English Version](README.md)
<br>

## Resumen De Comandos Para Realizar Commit Y Push Hacia Un Repositorio Remoto

    git init
    git add README.md
    git commit -m "first commit"
    git branch -M master
    git remote add origin [remote-repository]
    git push -u origin master
<br>

### Obtener Y Crear Proyectos

| Comando | Descripción |
| ------- | ----------- |
| `git init` | Inicializa un reporitorio Git local |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Crea una copia local de un repositorio remoto |
<br>

### Información Y Actualización

| Comando | Descripción |
| ------- | ----------- |
| `git status` | Verificar estado del repositorio |
| `git add [file-name.txt]` | Añadir un archivo |
| `git add -A` | Añadir todos los archivos nuevos y actualizados |
| `git commit -m "[commit message]"` | Hacer commit de los cambios realizados |
| `git rm -r [file-name.txt]` | Eliminar un archivo (ó folder) |
<br>

### Acciones Sobre Branch Y Merge

| Comando | Descripción |
| ------- | ----------- |
| `git branch` | Lista el branch (el asterisco denota el branch actual) |
| `git branch -a` | Lista todos los branches (locales y remotos) |
| `git branch [branch name]` | Crea un nuevo branch |
| `git branch -d [branch name]` | Borra un branch |
| `git push origin --delete [branch name]` | Borra un branch remoto |
| `git checkout -b [branch name]` | Cre un nuevo branch y se cambia a este |
| `git checkout -b [branch name] origin/[branch name]` | Clona un branch remoto y se cambia a este |
| `git branch -m [old branch name] [new branch name]` | Renombra un branch local |
| `git checkout [branch name]` | Cambiar a un branch específico |
| `git checkout -` | Cambia al último branch que se le realizó checkout |
| `git checkout -- [file-name.txt]` | Descarta los cambios de un archivo |
| `git merge [branch name]` | Combina un branch con el branch actual |
| `git merge [source branch] [target branch]` | Combina un branch con un branch específico |
| `git stash` | Guarda los cambios en un directorio de trabajo |
| `git stash clear` | Elimina todas las entradas escondidas |
<br>

### Actualizar Proyectos

| Comando | Descripción |
| ------- | ----------- |
| `git push origin [branch name]` | Realizar push a un branch del repositorio remoto |
| `git push -u origin [branch name]` | Realizar push a un branch del repositorio remoto (y recordar el branch) |
| `git push` | Realizar push a un branch del repositorio remoto (branch recordado) |
| `git push origin --delete [branch name]` | Borrar un branch remoto |
| `git pull` | Actualizar el repositorio local hacia el último commit |
| `git pull origin [branch name]` | Obtener los cambios del repositorio remoto |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Añadir un repositorio remoto |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Establecer el origen de un branch a SSH |
<br>

### Inspección y Comparación

| Comando | Descripción |
| ------- | ----------- |
| `git log` | Visualizar los cambios |
| `git log --summary` | Visualizar los cambios (detallados) |
| `git log --oneline` | Visualizar los cambios (resumidos) |
| `git diff [source branch] [target branch]` | Previsualizar los cambios antes de realizar merge |
<br>
