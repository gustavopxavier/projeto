----------------Logar no github pelo terminal-----------------

git config --global user.name "YOUR NAME"
git config --global user.email "YOUR EMAIL ADDRESS"

---------------Comandos para subir arquivos---------------
echo "# cartoriounico" >> README.md

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/gustavopxavier/projeto.git

git push -u origin master

--------------------Criar hg-pages------------------------

cd /pasta/do/projeto

git symbolic-ref HEAD refs/heads/gh-pages

rm .git/index

git clean -fdx

echo "Minha página no GitHub" > index.html

git add .

git commit -a -m "Primeiro commit de página no github"

git push origin gh-pages
