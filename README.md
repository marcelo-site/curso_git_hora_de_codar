# Principais Comandos do git

## git init

### Comandos principais

<b>git init</b>

Inicia um repositorio local

## git status

<b>Ele permite que você veja quais arquivos foram alterados desde o ultimo commit (arquivos traked com status modifed), quais não foram e quais arquivos não estão sendo rastreados pelo git (arquivos untracked).</b>

### Comandos principais

<b>git status </b>

Consultar quais arquivos foram alterados desde o ultimo commit (modifed) e quais foram adicionados (untracked)

## git pull

<b>Atualiza repositorio local de acordo com o repositório remoto</b>

### Comandos principais

<b>git pull</b>

atualiza repositório local de acordo com o repositório remoto

## git remote

<b>Conecta o repositório local com o repositório reomoto com seu addressRemote</b>

### Comandos principais

<b>git remote</b>

Lida com origens remotas (repositório remoto)

<b>git remote -v</b>

lista o a origem remoto atual

<b>git remote add origin "addresRemote"</b>

Adiciona origem remota indicando um endereço remoto indicado no botão "code" no repositório github

Exemplo de como conseguir um "addressRemote" no botão "code" no topo da pagina de um repositório especifico no github ao clicar fornece endereços para fazer clone esse endereço também serve como addressRemote

<b>git remote rm origin</b>

remove a origem remota adicionada anteriormente com "git remote add origin"

## git reset

<b>Reseta o repositorio local para a ultima versão do repositório remoto</b>

### Comandos principais

<b>git reset --hard origin nomeBranch</b>

Reseta o repositorio para a ultima versão do repositório remoto

## git rm

<b>Remove arquivos no fluxo do git falhando em arquivos com status untraked</b>

### Comandos principais

<b>git rm "fileNmae.txt"</b>

Remove arquivo "fileName.txt"

## git mv

<b>Move ou renomeia o arquivos</b>

### Comandos principais

<b>git mv "fileName.ext" "\*/fileName.ext"</b>

Move o arquivo "fileName.txt" par "\*/fileName.txt", ou apenas renomeia se os arquivos forem movidos no mesmo diretório

## git add

<b>Adiciona arquivos modificados a um estágio chamado Staged indicando que estao prontos para o commit</b>

### Comandos principais

<b> git add "fileName.ext"</b>

Adiciona o arquivo "fileName.ext", se ele tiver no status aterior ao commit (traked com status modifed ou untracked) para o estágio de commit.

<b>git add .</b>

Adiciona todos os arquivos que stiverem no fluxo do git(traked) com status "modifed" ou fora do fluxo do git(untracked) para o estágio que podem ser commitados.

## git commit

<b>Adicona arquivo para o estágio pronto para ser mandado para o repositório remoto com "git pull"</b>

### Comandos principais

## git commit -m

<b>Confirma todas as alterações de arquivos que estejam no fluxo do git (tacked) com status "modifed" e arquivos untraked e manda uma mensagem, se não estiver em staged ver "git add"</b>

## git commit -a -m

<b>Confirma todas as alterações em arquivos já no fluxo (arquivos tracked) sem a nescessidade de antes executar um "git add" e manda uma mensagem, ignora arquivos fora do fluxo do git (untracked)</b>

## git push

<b>Atualiza o repoistório remoto.</b>

### Cmandos prinicpais

<b>git push</b>

Envia os arquivos commitados do repositório local para o repoistório remoto.

## git branch

<b>Lida com branches (versões para separar desnvolvimentos paralelos ao principal).</b>

### Comandos principais

<b>git branch</b>

Lista as branchs atual do repositorio local

<b>git branch -d "nomeBranch"</b>

Deleta a branch local

<b>git push origin --delete nomeBracnh</b>

Deleta a branch "nomeBranch" do servidor (github)

## git checkout

<b>Responsável por gerenciar branchs</b>

### Comandos principais

<b>git checkout nomeBranch</b>

Cria a branch "nomeBranch"

<b>git checkout -b "nomeBranch"</b>

Cria branch e já seta este branch como atual

## git merge

<b>Responsável por unir branchs</b>

### Comandos principais

<b>git merge "nomeBranch"</b>

Une o branch atual com "nomeBranch"

<b>git merge origin/nomeBranch</b>

une o branch atual com "nomeBranch" do github

## git stash

<b>semelhante ao "git reset" mas, sem perda do código</b>

### Comandos principais

<b>git stash --hard origin nomeBranch</b>

Semelhante ao ## git reset mas, sem perda do código

<b>git stach list</b>

lista todas as stashs criados indexadas

<b>git stach apply index</b>

Recupera a stach desse index

<b>git stash show -p index</b>

Lista modificações do stach desse index

<b> git stash drop index</b>

Apaga stach desse index

<b>git stash clear</b>

Apaga todas as stachs

## git diff

<b>lista modificações feitas em arquivos</b>

### Comandos principais

<b>git diff</b>

Lista modificações feitas em todos arquivos

<b>git diff "fileName.ext"</b>

Lista modificações feitas no arquivo "filaeName.txt"

## git tag

<b>Responsável por criar um versionamento para branch a partir do momento que foi criada</b>

### Comandos principais

<b>git tag</b>

Lista todas as tags da branch atual

<b>git tag -a v1.0 -m "tagName" </b>

cria uma tag para branch atual um versionamento do codigo a partir do momento que é criada, acessando posteriormente pelo "tagName"

<b>git show "tagName"</b>

Lista detalhes da tag e modificações contidas no seu historico

<b>git push origin "tageName </b>

Envia a "tageName" para o repositório remoto

<b>git push origin --tags</b>

Envia todas as tags para o repositório remoto

## git fetch

<b>Lista todas os branchs do repositorio remoto e pode ser acessado por meio do git checkout nomeBranch </b>

### Comandos principais

<b>git fetch</b>

baixa todos os branchs do repositorio remoto e pode ser acessado por meio do git checkout "branchNmae"

## git submodule

<b>Um submodule é uma subdivisão do repositório que acrescentam outros repositorios dentro do prjeto, se o diretório atual for um submodule os comandos de git funcionam soment para o submodule.</b>

### Comandos principais

<b>git submodule</b>

lista todos os submodules do repositório

<b>git submodule add origin dirName</b>

adciona um submodulo ao diretorio "dirName"

<b>git push --recurse-submodules=on-demand</b>

atualiza o repositório do submodulo

## git show

<b>Serve para todas a alterações feitas em uma branch ou tag</b>

## Comandos principais

<b></b>
