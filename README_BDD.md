# Commandes Docker de Base

## Gestion des Conteneurs

- ```docker ps -a``` : Liste tous les conteneurs, y compris les conteneurs arrêtés.
- `docker run image_name` : Crée et démarre un conteneur à partir d'une image.
- `docker exec -it container_name bash` : Lance une session bash interactive dans un conteneur.
- `mysql -u root -p` : Lance une session prompt sql.
- `docker stop container_name` : Arrête un conteneur en cours d'exécution.
- `docker start container_name` : Démarre un conteneur arrêté.
- `docker restart container_name` : Redémarre un conteneur.
- `docker rm container_name` : Supprime un conteneur arrêté.

## Gestion des Images

- `docker images` : Liste toutes les images Docker présentes sur le système.
- `docker pull image_name` : Télécharge une image depuis un registre (comme Docker Hub).
- `docker rmi image_name` : Supprime une image Docker.
- `docker tag image_name new_tag` : Ajoute un nouveau tag à une image existante.

## Gestion des Logs et Inspecter

- `docker logs container_name` : Affiche les logs d'un conteneur.
- `docker inspect container_name` : Affiche les détails d'un conteneur ou d'une image (configuration, réseaux, etc.).

## Gestion des Réseaux et Volumes

- `docker network ls` : Liste les réseaux Docker.
- `docker volume ls` : Liste les volumes Docker.
- `docker network create network_name` : Crée un nouveau réseau Docker.
- `docker volume rm volume_name` : Supprime un volume Docker.

# Commandes Docker Compose de Base

- `docker-compose up -d` : Démarre les conteneurs définis dans `docker-compose.yml` en arrière-plan.
- `docker-compose down` : Arrête et supprime tous les conteneurs, réseaux et volumes associés à un projet Docker Compose.
- `docker-compose logs -f` : Affiche les logs en temps réel des services gérés par Docker Compose.
- `docker-compose stop` : Arrête tous les conteneurs sans les supprimer.
- `docker-compose exec service_name command` : Exécute une commande dans un conteneur d'un service spécifique.

