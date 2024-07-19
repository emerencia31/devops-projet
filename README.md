# *devops-projet*

Nous allons configurer des tests automatiques qui s'exécutent à chaque push sur la branche principale du repository GitHub  et Construire un conteneur Docker : À chaque changement réussi et test passé, construire une image Docker de l'application web.


# creer un repository

Ajoute tous les fichiers du projet au dépôt : git add .

Faire un commit de nos fichiers : git commit -m "Initial commit"

Ajoutez le repository GitHub : git config --global user.email "33767@Regis-tchicaya"

Poussez le projet local vers GitHub :git push -u origin master

# Faire les tests
Nous allons ajouter une structure de tests avec Jest.
npm init -y
npm install jest --save-dev


# Dockerfile

Construire l'image Docker : docker build -t devops-projet.


Exécuter le conteneur à partir de l'image de nginx : docker run -d -p 8080:80 devops-projet

# Configurer GitHub Actions
Creation d'un dossier .github/workflows puis on  ajoute un fichier ci.yml :

Ajoute nos secrets Docker Hub à GitHub Actions :

Allez dans les "Settings" de notre repository.
Clique sur "Secrets and variables" puis "Actions".
Ajoute DOCKER_USERNAME et DOCKER_PASSWORD.


Accédez à l'application via l'adresse: http://localhost:8080.
