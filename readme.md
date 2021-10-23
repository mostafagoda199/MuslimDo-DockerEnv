# To install project
    1.install docker 
    2.install docker-composer
    
# Clone this repo
    git clone https://github.com/mostafagoda199/LampEnvWithDocker.git

# Repair your env
    make dir with name www
    rename .env-sample to .env
    rename docker-compose-sample.yml to docker-compose.yml

# Up docker images
    run "docker compose up -d" 

# Rebuild docker images
    run "docker compose up -d --no-deps --build" 

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
