# TP-IGL-Front-End 

## Lancer l'application Localement : 

Pour lancer l'application en local installer NodeJS et Git , aprés éxecutez ces commandes : 

1. Cloner le repository :

`git clone https://github.com/AbdelkhalekESI/TP-IGL-Client`

2. Installer les dépendances :

`npm install`

3. Lancer l'application :

`npm run serve`

4. Accéder à l'application via : `http://127.0.0.1:8080`

## Lancer l'application en utilisant Docker : 

Pour lancer l'application en local installer Docker et Git ,aprés éxecutez ces commandes : 

1. Cloner le repository :

`git clone https://github.com/AbdelkhalekESI/TP-IGL-Client`

2. Construire l'image Docker : 

`docker build -t tp-igl/vue-app:0.1 .`

3. Lancer le conteneur Docker : 

`docker run -it -p 8080:8080 --rm tp-igl/vue-app:0.1`

4. Accéder à l'application via : `http://127.0.0.1:8080`
