Comandos Git
============

## Versiones Traducidas
- [Versión en Inglés](README.md)
<br>

## Resumen de comandos para realizar commit y push hacia un repositorio remoto

    git init
    git add README.md
    git commit -m "[mensage del commit]"
    git branch -M master
    git remote add origin [repositorio-remoto]
    git push -u origin master
<br>

### Obtener Y Crear Proyectos

| Comando | Descripción |
| ------- | ----------- |
| `git init` | Inicializa un reporitorio Git local |
| `git clone ssh://git@github.com/[nombreDeUsuario]/[nombreDelRepositorio].git` | Crea una copia local de un repositorio remoto |
<br>

### Información Y Actualización

| Comando | Descripción |
| ------- | ----------- |
| `git status` | Verificar estado del repositorio |
| `git add [nombreDelArchivo.txt]` | Añadir un archivo |
| `git add -A` | Añadir todos los archivos nuevos y actualizados |
| `git commit -m "[mensage del commit]"` | Hacer commit de los cambios realizados |
| `git rm -r [nombreDelArchivo.txt]` | Eliminar un archivo (ó folder) |
<br>

### Acciones Sobre Branch Y Merge

| Comando | Descripción |
| ------- | ----------- |
| `git branch` | Lista el branch (el asterisco denota el branch actual) |
| `git branch -a` | Lista todos los branches (locales y remotos) |
| `git branch [nombreDelBranch]` | Crea un nuevo branch |
| `git branch -d [nombreDelBranch]` | Borra un branch |
| `git push origin --delete [nombreDelBranch]` | Borra un branch remoto |
| `git checkout -b [nombreDelBranch]` | Cre un nuevo branch y se cambia a este |
| `git checkout -b [nombreDelBranch] origin/[nombreDelBranch]` | Clona un branch remoto y se cambia a este |
| `git branch -m [nombreDelBranchViejo] [nombreDelBranchNuevo]` | Renombra un branch local |
| `git checkout [nombreDelBranch]` | Cambiar a un branch específico |
| `git checkout -` | Cambia al último branch que se le realizó checkout |
| `git checkout -- [nombreDelArchivo.txt]` | Descarta los cambios de un archivo |
| `git merge [nombreDelBranch]` | Combina un branch con el branch actual |
| `git merge [nombreDelBranchFuente] [nombreDelBranchObjetivo]` | Combina un branch con un branch específico |
| `git stash` | Guarda los cambios en un directorio de trabajo |
| `git stash clear` | Elimina todas las entradas escondidas |
<br>

### Actualizar Proyectos

| Comando | Descripción |
| ------- | ----------- |
| `git push origin [nombreDelBranch]` | Realizar push a un branch del repositorio remoto |
| `git push -u origin [nombreDelBranch]` | Realizar push a un branch del repositorio remoto (y recordar el branch) |
| `git push` | Realizar push a un branch del repositorio remoto (branch recordado) |
| `git push origin --delete [nombreDelBranch]` | Borrar un branch remoto |
| `git pull` | Actualizar el repositorio local hacia el último commit |
| `git pull origin [nombreDelBranch]` | Obtener los cambios del repositorio remoto |
| `git remote add origin ssh://git@github.com/[nombreDeUsuario]/[nombreDelRepositorio].git` | Añadir un repositorio remoto |
| `git remote set-url origin ssh://git@github.com/[nombreDeUsuario]/[nombreDelRepositorio].git` | Establecer el origen de un branch a SSH |
<br>

### Inspección y Comparación

| Comando | Descripción |
| ------- | ----------- |
| `git log` | Visualizar los cambios |
| `git log --summary` | Visualizar los cambios (detallados) |
| `git log --oneline` | Visualizar los cambios (resumidos) |
| `git diff [nombreDelBranchFuente] [nombreDelBranchObjetivo]` | Previsualizar los cambios antes de realizar merge |
<br>
