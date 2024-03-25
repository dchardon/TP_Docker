Etape 2: Utilisation de docker compose
Utilisez docker compose pour déployer vos 4 services nginx et votre loadbalancer.

Sur le terminal : se rendre dans le dossier où se trouve le fichier compose.yaml
docker compose « nom_du_fichier » up

Etape 3: Dockeriser une application existante
Nous souhaitons partir d'une application Web de détection de visage.
Src dans ce repository
https://github.com/barais/TPDockerSampleApp

Construisez le fichier docker file permettant de créer l'image docker pour cette application.
Télécharger le zip de l’application et l’extraire. Créer un Dockerfile.

Sur le terminal : se rendre dans le dossier où se trouve le Dockerfile
Compiler du image : docker build .
Afficher toutes les images : docker image ls
Renommer une image : docker tag « id » « nom_app »
Executer l’application : docker run -p « port à exposer»:8080 -t -i « nom_app »

Supprimer un container : docker rm « id »
Supprimer une image : docker image rm « id »
