

UID_GID="$(id -u):$(id -g)" docker-compose up -d

sudo chown -R $USER:$USER /opt/www

docker exec -it php7.4 sh

docker exec -it php8.0 sh

UID_GID="$(id -u):$(id -g)" docker-compose down


take backup of db while shutting down docker