# *devops-projet*

Nous allons configurer des tests automatiques qui s'exécutent à chaque push sur la branche principale du repository GitHub  et Construire un conteneur Docker : À chaque changement réussi et test passé, construire une image Docker de l'application web.


# creer un repository

Ajoutez tous les fichiers de votre projet au dépôt : git add .

Faire un commit de vos fichiers : git commit -m "Initial commit"

Ajoutez le repository GitHub : git config --global user.email "33767@Regis-tchicaya"

Poussez votre projet local vers GitHub :git push -u origin master

# Creer les fichiers de l'application : index.html , style.css et scritp.js


# Faire les tests
Nous allons ajoutez une structure de tests avec Jest.
npm init -y
npm install jest --save-dev


# Dockerfile

Construire l'image Docker : docker build -t devops-projet.


Exécuter le conteneur à partir de l'image de nginx : docker run -d -p 8080:80 devops-projet

# structure du repertoire
── Dockerfile
── index.html
── script.js
── styles.css
── test.js

# Accédez à l'application via l'adresse: http://localhost:8080.
