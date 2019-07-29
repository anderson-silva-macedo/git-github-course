Principais comandos do git

configuração inicial git

git config --global user.name "user name";
git config --global user.email "user@email.com";
git config -l => lista todas opções disponiveis

git config --global core.excludesfile ~/.gitignore => ele irá configurar de forma global todos arquivos ignorados em todos os projetos na nossa maquina sem a necessidade de ficarmos incluindo tem todos os projetos

git init => inicia um repositorio local

git status => verifica o estado dos documentos do seu repositorio local

git add { git add . ou git add index.html style.css} => adiciona o arquivo de local do work directory=> para stage area

git add --all ou git add -A => adiciona todos tipos de status de arquivos

git rm { git rm style.css } => remove um arquivo do git directory, depois fazemos um commit -m "msg" para remover o arquivo definitivo

git rm -r { git rm -r node_modules }=> remove um diretorio definitivo

git rm -rf nome_modules/ --cached ou { git rm nome_aquivo --cached} => remove do git mais não apaga ele do nosso diretorio local ou seja recupera da stage area para o working directory

git commit -m "msg" => adiciona arquivos de stage area para => .git directory repository

git commit -a -m "msg" ou usar { -am "msg" }=> adiciona arquivos e ja comitamos juntos

git log => mostra o commit completo => hash,author,email,data,e msg de commit

git log --name-status => mostra o comit com detalhes se "A" adicionado, "M" modificado ou "D" deletado

git log --pretty=oneline => mostra hash do commit e a mensagem do commit

git log --abbrev-commit => abrevia o hash do commit ( podemos juntar parametros: exemplo git log --pretty=oneline --abbrev-commit )

git log --stat => mostra algumas estatisticas do nosso log

git log -p => mostra o que foi alterado nesse arquivo

git log -p -3 => mostra o que foi alterado nesse arquivo o -3 serve para mostrar apenas os 3 últimos

git diff => usado para verificar as diferenças do arquivo antes de add a stage area

git diff --staged => usado para verificar as diferenças do arquivo na stage area antes de commit => git directory respository

git diff 0efda736c53e089098119c5ebebbcee58d217c2d => mostra a diferença de um hash para o seu commit atual

git diff 0efda736c53e089098119c5ebebbcee58d217c2d 0efda736c53e089098119c5ebebbcee58d217c2d => mostra diferença de um hash para outro

git branch => lista as branchs disponiveis (ou seja as ramificações)

git branch nome_branch => cria uma branch nova

git branch -m novo_nome => renomeia a branch atual que estamos

git branch -D nome_branch => deleta branch

git checkout nome_branch => muda de branch

git checkout -b nome_branch => cria uma branch com o nome descrito e já muda para esta branch

git checkout --oprphan nome_branch => cria uma branch nova vazia

git merge nome_branch => unifica todos os arquivos e diretorios
























