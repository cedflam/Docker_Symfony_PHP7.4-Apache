# Docker Template

### Configuration Postgres :
* Modifier postgresql.conf -> 'listen_addresses' = '*'
* Modifier pg_hba.conf -> 'host all all 192.168.1.0/24 trust'

####Attention ! Effectuer les paramétrages nécessaires des fichiers :
* docker-compose.yml
* Dockerfile
* vhosts.conf

### Installation de Docker :
* Installer docker 
* cmd -> docker-compose up -d (Télécharge les images et lance les containers)
* cmd -> docker exec -it container_name bash (Pour entrer dans le container)
* cmd -> cd project (Entrer dans le dossier du projet)
* cmd -> git clone project (récupère le repo Git)
* cmd -> composer install (installe les dépendances Symfony) 
* cmd -> npm install (Installe les dépendances NodeJs)
* cmd -> npm run build (Construit les fichiers de prod Node React)
 