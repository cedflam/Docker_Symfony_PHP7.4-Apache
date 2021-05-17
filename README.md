# Docker Template

### Configuration Postgres (Bdd sur machine locale):
* Modifier postgresql.conf -> 'listen_addresses' = '*'
* Modifier pg_hba.conf -> 'host all all 192.168.1.0/24 trust'

### Attention ! Effectuer les paramétrages nécessaires des fichiers :
* docker-compose.yml
* Dockerfile
* vhosts.conf (modifier le chemin vers l'application)

### Installation de Docker :
* Installer docker 
* cmd -> docker-compose up -d (Télécharge les images et lance les containers)
* cmd -> docker exec -it container_name bash (Pour entrer dans le container)
* cmd -> cd project (Entrer dans le dossier du projet)
* cmd -> git clone project (récupère le repo Git)
* cmd -> composer install (installe les dépendances Symfony) 
* cmd -> npm install (Installe les dépendances NodeJs)
* cmd -> npm run build (Construit les fichiers de prod Node React)

### Exemple de .env fichiers avec bdd multiple
DATABASE_URL="postgresql://postgres:root@192.168.1.47:5432/postgres?serverVersion=13&charset=utf8"
DATABASE_INTRANET_URL="postgresql://postgres:root@192.168.1.47:5432/intranet?serverVersion=13&charset=utf8"
 