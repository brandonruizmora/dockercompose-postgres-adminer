# Docker-compose 

commands to use in docker-compose.yml and stack.yml
Define and run multi-container applications with Docker


#### Define 2 files 
    - docker-compose.yml
    - stackdb.yml


### To pull images of DB: postgres and UI: adminer

docker-compose pull (This command will execute file docker-compose.yml)

docker-compose -f stackdb.yml pull (This command will execute file stackdb.yml)


### Build, (re)creates, starts containers based on images defined in yml file

docker-compose up -d (This command will Build, (re)creates, starts 2 containers based on docker-compose.yml in background mode)
docker-compose -f stackdb.yml up -d (This command will Build, (re)creates, starts 2 containers based on stackdb.yml in background mode)