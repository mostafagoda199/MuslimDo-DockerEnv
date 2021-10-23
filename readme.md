# To install project
    1.install docker 
    2.install docker-composer
# change Owner Role add to the end of file  /bin/php$(v) 
    RUN chown $(user) /var/www/html
    USER $(user)
    
# Up docker images
    docker compose up -d

# Rebuild docker images
    docker compose up -d --no-deps --build

# Down docker images
    sudo docker-compose down

# List docker Containers
    docker container ls -a
    docker ps -a 

# List docker images
    docker images -q

# Execute docker images
    sudo docker exec -it $container_name bash

# Remove All Containers
    docker -rm -f $(docker ps -a -q)

# Remove All images
    docker -rmi -f $(docker images -a -q)

# Show Logs 
     docker-compose logs
