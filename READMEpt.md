Comandos Git
============

_Uma lista dos comandos Git mais usados_

*Se voc� est� interessado em meus aliases do Git, d� uma olhada no meu `.bash_profile`, encontrado aqui: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Obtendo & Cria��o de Projetos

| Comando | Descri��o |
| ------- | --------- |
| `git init` | Inicializa um reposit�rio Git local |
| `git clone ssh://git@github.com/[usuario]/[nome-repositorio].git` | Cria uma c�pia local de um reposit�rio remoto |

### B�sicos

| Comando | Descri��o |
| ------- | --------- |
| `git status` | Checa o status |
| `git add [nome-arquivo.txt]` | Adiciona um arquivo para �rea de stage |
| `git add -A` | Adiciona todos os arquivos novos ou modificados para a �rea de stage |
| `git commit -m "[Mensagem de Commit]"` | Comita as altera��es |
| `git rm -r [nome-arquivo.txt]` | Remove um arquivo (ou pasta) |

### Branching & Merging

| Comando | Descri��o |
| ------- | --------- |
| `git branch` | Lista as branches (o asterisco denota a branch atual) |
| `git branch -a` | Lista todas as branches (local e remoto) |
| `git branch [nome da branch]` | Cria uma nova branch |
| `git branch -d [nome da branch]` | Deleta uma branch |
| `git push origin --delete [nome da branch]` | Deleta uma branch remota |
| `git checkout -b [nome da branch]` | Cria uma nova branch e muda para ela |
| `git checkout -b [nome da branch] origin/[nome da branch]` | Clona uma branch remota e muda para ela |
| `git checkout [nome da branch]` | Seleciona uma branch |
| `git checkout -` | Muda para a �ltima branch |
| `git checkout -- [nome-arquivo.txt]` | Descarta modifica��es de um arquivo |
| `git merge [nome da branch]` | Faz um merge de uma branch na branch atual |
| `git merge [source branch] [branch alvo]` | Faz um merge de uma branch em outra branch |
| `git stash` | Tirar o estado sujo do seu diret�rio de trabalho |
| `git stash clear` | Remove todas as entradas 'stash' |

### Sharing & Updating Projects

| Comando | Descri��o |
| ------- | --------- |
| `git push origin [nome da branch]` | Enviar uma branch para seu reposit�rio remoto |
| `git push -u origin [nome da branch]` | Envia as altera��es da branch informada para um reposit�rio remoto (and selecionar a branch) |
| `git push` | Envia as altera��es para o reposit�rio remoto (branch atual) |
| `git push origin --delete [nome da branch]` | Deletar uma branch remota |
| `git pull` | Atualiza o reposit�rio local para o �ltimo commit |
| `git pull origin [nome da branch]` | Recebe altera��es do reposit�rio remoto |
| `git remote add origin ssh://git@github.com/[usuario]/[nome-repositorio].git` | Adicionar um reposit�rio remoto |
| `git remote set-url origin ssh://git@github.com/[usuario]/[nome-repositorio].git` | Seta um reposit�rio da origin branch para o SSH |

### Inspe��o & Compara��o

| Comando | Descri��o |
| ------- | --------- |
| `git log` | Ver modifica��es |
| `git log --summary` | Ver modifica��es (detalhadas) |
| `git diff [branch original] [branch alvo]` | Visualizar altera��es antes de mesclar |

