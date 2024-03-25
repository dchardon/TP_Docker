Etape 2: Utilisation de docker compose

Sur le terminal : se rendre dans le dossier où se trouve le fichier compose.yaml
docker compose « nom_du_fichier » up

Etape 3: Dockeriser une application existante
Télécharger le zip de l’application et l’extraire. Créer un Dockerfile.

Sur le terminal : se rendre dans le dossier où se trouve le Dockerfile
Compiler du image : docker build .
Afficher toutes les images : docker image ls
Renommer une image : docker tag « id » « nom_app »
Executer l’application : docker run -p « port à exposer»:8080 -t -i « nom_app »

Supprimer un container : docker rm « id »
Supprimer une image : docker image rm « id »
