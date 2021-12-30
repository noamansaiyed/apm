

UID_GID="$(id -u):$(id -g)" docker-compose up -d

sudo chown -R $USER:$USER /opt/www

docker exec -it php74 sh

UID_GID="$(id -u):$(id -g)" docker-compose down