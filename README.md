Partie A : Création d'un Serveur HTTP Minimaliste avec Docker

1. Construire l'image Docker
docker build -t basic-http-server .

2. Lancer le conteneur
docker run -p 8000:8000 basic-http-server

3. Lancer le conteneur avec Docker Compose
docker-compose up --build



Partie B : Pousser l’image de l’application vers DockerHub 

1. Construire une image Docker de l'application.
docker build -t basic-http-server .

2. Se connecter à DockerHub via la ligne de commande
docker login

3. Taguer l’image Docker pour qu’elle soit prête à être poussée sur DockerHub
docker tag basic-http-server adams365/basic-http-server:latest
docker tag basic-http-server adams365/basic-http-server:v1.0

4. Pousser l’image sur DockerHub pour la rendre accessible en ligne
docker push adams365/basic-http-server:latest
docker push adams365/basic-http-server:v1.0
#   b a s i c _ s e r v e r  
 