# devops-projet
Nous allons configurer des tests automatiques qui s'exécutent à chaque push sur la branche principale du repository GitHub  et Construire un conteneur Docker : À chaque changement réussi et test passé, construire une image Docker de l'application web.

-Tests
Nous allons ajoutez une structure de tests avec Jest.
npm init -y
npm install jest --save-dev

-Dockerfile
Construisez l'image Docker :
docker build -t devops-projet.


Exécutez un conteneur à partir de l'image :
docker run -d -p 8080:80 simple-web-app


Accédez à l'application vial'adresse: http://localhost:8080.
