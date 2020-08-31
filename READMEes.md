Comandos Git
============

## Versiones Traducidas
- [English Version](README.md)
<br>

## Resumen de comandos para realizar commit y push hacia un repositorio remoto

    git init
    git add README.md
    git commit -m "first commit"
    git branch -M master
    git remote add origin [remote-repository]
    git push -u origin master
<br>

### Obtener y crear proyectos

| Comando | Descripción |
| ------- | ----------- |
| `git init` | Inicializa un reporitorio Git local |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Crea una copia local de un repositorio remoto |
<br>

### Información y actualización

| Comando | Descripción |
| ------- | ----------- |
| `git status` | Verificar estado del repositorio |
| `git add [file-name.txt]` | Añadir un archivo |
| `git add -A` | Añadir todos los archivos nuevos y actualizados |
| `git commit -m "[commit message]"` | Hacer commit de los cambios realizados |
| `git rm -r [file-name.txt]` | Eliminar un archivo (ó folder) |
<br>

### Acciones sobre branches y merge

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

### Sharing & Updating Projects

| Comando | Descripción |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |
<br>

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |
<br>
