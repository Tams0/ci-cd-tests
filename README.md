--Création du package.json file
npm init

--Initialisation d'un dépot Git vide dans C:/Users/Tamso/ci-cd-tests/.git/
git init

--Add et push des modifications
git remote add origin https://github.com/Tams0/ci-cd-tests.git
git branch -M main
git push -u origin main
git add .
git config --global user.email "lioneltamo237@gmail.com"
git config --global user.name "Tams0"
git commit -m "Premier commit"
git push -u origin main

--Initialisation de express(toutes les dépenances du projet seront ici dans node_modules)
npm install express

--Installation de trois librairies jest supertest et eslint en version 8, les dépendances de dev
npm install --save-dev jest supertest eslint@8 

--Lancement de notre serveur
node src/app.js
