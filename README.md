# Setting up of pgAdmin 4 using official docker image
This repository is used for setting up pgAdmin for administering postgres database.

## Setup
- [pgAdmin 4 v4.6](https://hub.docker.com/r/dpage/pgadmin4/ "pgAdmin Official Docker Image")
- Docker 18.05.0-ce 
- Docker-compose 1.21.2

## Running it
- Pull the official image from docker hub
    - `docker pull dpage/pgadmin4:4.6`
- With the docker-compose file in the same directory,
    - To start, `docker-compose up -d` 
    - To stop, `docker-compose down `
    
## Removing previous version
- Stop the container
    - `docker stop 'containerid'`
- Show all container and remove container accordingly
    - `docker container ls --all`
    - `docker container rm 'containerid`
- Remove the image
    - `docker image ls --all`
    - `docker image rm 'imageid'`
    