# Principais Comandos do git

## git init

<b>Inicia u repositorio local</b>

### Comandos principais

#### git init

Inicia um repositorio local

## git status

<b> Ele permite que você veja quais arquivos foram alterados desde o ultimo commit (arquivos traked com status modifed), quais não foram e quais arquivos não estão sendo rastreados pelo git (arquivos untracked).</b>

### Comandos principais

#### git status

Consultar quais arquivos foram alterados desde o ultimo commit (modifed) e quais foram adicionados (untracked)

## git pull

<b>Atualiza repositorio local de acordo com o repositório remoto</b>

### Comandos principais

#### git pull

atualiza repositório local de acordo com o repositório remoto

## git remote

<b>Conecta o repositório local com o repositório reomoto com seu addressRemote</b>

### Comandos principais

#### git remote

Lida com origens remotas (repositório remoto)

#### git remote -v

lista o a origem remoto atual

#### git remote add origin "addresRemote"

Adiciona origem remota indicando um endereço remoto indicado no botão "code" no repositório github

Exemplo de como conseguir um "addressRemote" no botão "code" no topo da pagina de um repositório especifico no github ao clicar fornece endereços para fazer clone esse endereço também serve como addressRemote

#### git remote rm origin

remove a origem remota adicionada anteriormente com "git remote add origin"

## git reset

<b>Reseta o repositorio local para a ultima versão do repositório remoto</b>

### Comandos principais

#### git reset --hard origin nomeBranch

Reseta o repositorio para a ultima versão do repositório remoto

## git rm

<b>Remove arquivos no fluxo do git falhando em arquivos com status untraked</b>

### Comandos principais

#### git rm "fileNmae.txt"

Remove arquivo "fileName.txt"

## git mv

<b>Move ou renomeia o arquivos</b>

### Comandos principais

#### git mv "fileName.ext" "\*/fileName.ext"

Move o arquivo "fileName.txt" par "\*/fileName.txt", ou apenas renomeia se os arquivos forem movidos no mesmo diretório

## git add

<b>Adiciona arquivos modificados a um estágio chamado Staged indicando que estao prontos para o commit</b>

### Comandos principais

#### git add "fileName.ext"

Adiciona o arquivo "fileName.ext", se ele tiver no status aterior ao commit (traked com status modifed ou untracked) para o estágio de commit.

#### git add .

Adiciona todos os arquivos que stiverem no fluxo do git(traked) com status "modifed" ou fora do fluxo do git(untracked) para o estágio que podem ser commitados.

## git commit

<b>Adicona arquivo para o estágio pronto para ser mandado para o repositório remoto com "git pull"</b>

### Comandos principais

#### git commit -m

Confirma todas as alterações de arquivos que estejam no fluxo do git (tacked) com status "modifed" e arquivos untraked e manda uma mensagem, se não estiver em staged ver "git add"

#### git commit -a -m

Confirma todas as alterações em arquivos já no fluxo (arquivos tracked) sem a nescessidade de antes executar um "git add" e manda uma mensagem, ignora arquivos fora do fluxo do git (untracked)

#### git push

Atualiza o repoistório remoto.

## git push

Atualiza o repositrio remoto

### Comandos prinicpais

#### git push

Envia os arquivos commitados do repositório local para o repoistório remoto.

## git branch

<b>Lida com branches (versões para separar desnvolvimentos paralelos ao principal).</b>

### Comandos principais

#### git branch

Lista as branchs atual do repositorio local

#### git branch -d "branchName"

Deleta a branch local "branchName"

#### git push origin --delete "branchName"

Deleta a branch "branchName" do repoistório remoto

## git checkout

<b>Responsável por criar e setar branchs</b>

### Comandos principais

#### git checkout "branchName"

Cria a branch "branchName"

#### git checkout -b "branchName"

Cria branch e já seta este branch como atual

## git merge

<b>Responsável por unir branchs</b>

### Comandos principais

#### git merge "nomeBranch"

Une o branch atual com "nomeBranch"

#### git merge origin/nomeBranch

une o branch atual com "nomeBranch" do github

## git stash

<b>Semelhante ao "git reset" mas, sem perda do código.</b>

### Comandos principais

#### git stash --hard origin nomeBranch

Semelhante ao ## git reset mas, sem perda do código

#### git stach list

lista todas as stashs criados indexadas

#### git stach apply index

Recupera a stach desse index

#### git stash show -p index

Lista modificações do stach desse index

#### git stash drop index

Apaga stach desse index

#### git stash clear

Apaga todas as stachs

## git diff

<b>Lista modificações feitas em arquivos</b>

### Comandos principais

#### git diff

Lista modificações feitas em todos arquivos

#### git diff "fileName.ext"

Lista modificações feitas no arquivo "filaeName.txt"

## git tag

<b>Responsável por criar um versionamento para branch a partir do momento que foi criada.</b>

### Comandos principais

#### git tag

Lista todas as tags da branch atual

#### git tag -a v1.0 -m "tagName"

cria uma tag para branch atual um versionamento do codigo a partir do momento que é criada, acessando posteriormente pelo "tagName"

#### git show "tagName"

Lista detalhes da tag e modificações contidas no seu historico

#### git push origin "tagName"

Envia a "tagName" para o repositório remoto

#### git push origin --tags

Envia todas as tags para o repositório remoto

## git fetch

<b>Lista todas os branchs do repositorio remoto e pode ser acessado por meio do git checkout nomeBranch</b>

### Comandos principais

#### git fetch

baixa todos os branchs do repositorio remoto e pode ser acessado por meio do git checkout "branchNmae"

## git submodule

<b>Um submodule é uma subdivisão do repositório que acrescentam outros repositorios dentro do prjeto, se o diretório atual for um submodule os comandos de git funcionam soment para o submodule.</b>

### Comandos principais

#### git submodule

lista todos os submodules do repositório

#### git submodule add origin dirName

adciona um submodulo ao diretorio "dirName"

#### git push --recurse-submodules=on-demand

atualiza o repositório do submodulo

## git show

<b>Serve para todas a alterações feitas em uma branch ou tag</b>

## Comandos principais

####
