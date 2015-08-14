cd /pasta/do/projeto
git symbolic-ref HEAD refs/heads/gh-pages
rm .git/index
git clean -fdx
echo "Minha página no GitHub" > index.html
git add .
git commit -a -m "Primeiro commit de página no github"
git push origin gh-pages
