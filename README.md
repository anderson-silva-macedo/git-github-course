Comandos basicos

configuracao inicial

git config --global user.name "Anderson"
git config --global user.email "andersonmacedo1782@hotmail.com"
git config --global core.editor code .
git config --list

git init //iniciar repositorio "untracked"
git status //mostra arquivos modificados 
git add nome arquivo //adiciona ao git "stage area"
git rm nome arquivo //remove ao git "stage area"
git commit -m "msg" //adiciona ao "stage repository"
git log //mostra informacoes
git log --decorate //mostra informacoes e qual branch
git log --author "nome pessoa"
git shortlog //mostra resumo