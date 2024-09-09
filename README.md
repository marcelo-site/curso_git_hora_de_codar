# Principais Comandos do git

## git init

<b>descrição: </b> inicia um repositorio local.

## git remote add origin "remote address"

<b>descrição: </b> adiciona origem remota indicando um endereço remoto indicado no botão "code" no repositório github

## git remote -v

<b>descrição: </b> lista o a origem remoto atual.

## git remote

<b>descrição: </b> lista origens remota

## git remote rm origin

<b>descrição: </b> remove a origem remota

## git status

<b>descrição: </b> consultar status.

## git pull

<b>descrição: </b> atualiza repositorio local de acordo com o github

## git reset --hard origin nomeBranch

<b>descrição: </b> reseta o repositorio para a ultima versão do ## github

## git rm file.ext

<b>descrição: </b> remove arquivo

## git mv file.ext dest/\*.ext

<b>descrição: </b> move ou renomeia o arquivo

## git add file.txt

<b>descrição: </b> adiciona o arquivo file.ext modificafo.

## git add .

<b>descrição: </b> adiciona todos arquivos modificados.

## git commit

<b>descrição: </b> adicona alteração

## git commit -a -m

<b>descrição: </b> confirmar todas as alterações e manda uma mensagem

## git push

<b>descrição: </b> envia o estado atual do repositório local para o github, mas só os commitados

## git branch

<b>descrição: </b> lista as branchs atual do repositorio local

## git branch -d nomeBranch

<b>descrição: </b> deleta a branch local

## git push origin --delete nomeBracnh

<b>descrição: </b> deleta a branch "nomeBranch" do ## github

## git checkout nomeBranch

<b>descrição: </b> cria a branch "nomeBranch"

## git checkout -b nomeBranch

<b>descrição: </b> cria branch e já seta este branch como atual

## git merge nomeBranch

<b>descrição: </b> une o branch atual com "nomeBranch"

## git merge origin/nomeBranch

<b>descrição: </b> une o branch atual com "nomeBranch" do github

## git stash --hard origin nomeBranch

<b>descrição: </b> semelhante ao ## git reset mas, sem perda do código

## git stach list

<b>descrição: </b> lista todas as stashs criados indexadas

## git stach apply index

<b>descrição: </b> recupera a stach desse index

## git stash show -p index

<b>descrição: </b> lista modificações do stach desse index

## git diff

<b>descrição: </b> lista modificações feitas em todos arquivos

## git stash drop index

<b>descrição: </b> apaga stach desse index

## git stash clear

<b>descrição: </b> apaga todas as stach

## git diff file.ext

<b>descrição: </b> lista modificações feitas no arquivo

## git tag -a v1.0 -m "tag v1.0"

<b>descrição: </b> cria uma tag para branch atual um versionamento do codigo a partir do momento que é cridao

## git tag

<b>descrição: </b> lista todas as tags da branch atual

## git show nameTag

<b>descrição: </b> lista detalhes da tag e modificações contidas no seu historico

## git push origin nameTag

<b>descrição: </b> envia para o servidor a tag

## git push origin --tags

<b>descrição: </b> envia para o servidor toas tags

## git fetch

<b>descrição: </b> baixa todos os branchs do repositorio no ## github e pode ser acessado por meio do ## git checkout nomeBranch

## git submodule

<b>descrição: </b> Lista os submodulos

## git submodule

<b>descrição: </b> um submodule é uma subdivisão do repositório que acrescentam outros repositorios dentro do prjeto, se o diretório atual for um submodule os comandos de git funcionam soment para o submodule.

### Comandos

<b>git submodule</b>
lista todos os submodules do repositório

<b>git submodule add origin dirName</b>
adciona um submodulo ao diretorio "dirName"

<b>git push --recurse-submodule=on-demand</b>
atualiza o submodulo
