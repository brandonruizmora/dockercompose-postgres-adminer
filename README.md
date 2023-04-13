# Docker-compose 

## Required

- Docker desktop [Download link](https://docs.docker.com/get-docker/)

### or

- Docker ubuntu

Uninstall older versions
` sudo apt-get remove docker docker-engine docker.io containerd runc`

Install last version
`sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin`

---

**_commands to use in docker-compose.yml and stack.yml_**

**_Define and run multi-container applications with Docker_**


#### Define 2 files 
    - docker-compose.yml
    - stackdb.yml


### To pull images of DB: postgres and UI: adminer

docker-compose pull (This command will execute file docker-compose.yml)

docker-compose -f stackdb.yml pull (This command will execute file stackdb.yml)


### Build, (re)creates, starts containers based on images defined in yml file

docker-compose up -d (This command will Build, (re)creates, starts 2 containers based on docker-compose.yml in background mode)
docker-compose -f stackdb.yml up -d (This command will Build, (re)creates, starts 2 containers based on stackdb.yml in background mode)
