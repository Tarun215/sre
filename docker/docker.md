# Docker Learning Objectives

## What are containers?
- Container are completely isolated environments (as in they can have their own processes or services, thier own network interfaces, their own mounts just like VM's except they all share the same os kernel)
- Some of different types of containers are:
    - LXC
    - LXD
    - LXCFS
    etc.
- Docker utilizes LXC's
- Setting up these container environments is hard as they are very low-level. (That is what docker provides us, a high level tool to create containers)

## What is docker?

## Why do you need docker?

## What can it do?
- Containerize applications
- Run each service with its own dependencies in seprate containers


## Docker Commands
- **Docker run** - start a container
```
docker run <image>
```
This command will run an instance of application defined in image
- **Docker ps** - list containers
```    
docker ps
```
list all running containers and some basic information about them
```
docker ps -a
```
list all containers running or not
- **Docker stop** - stop container
```
docker stop <container_name or container_id>
```
stops given container
- **Docker rm** - remove container
```
docker rm <container_name>
```
to remove a stopped or exited container permanently
- **Docker images** - list images
```
docker images
```
to list images present on host
- **Docker rmi** - remove image
```
docker rmi <image>
```
removes image from local, *MUST* ensure that no container is running on that image
- **Docker pull** - download image
```
docker pull <image>
```
downloads image and stores it on our host
- **Docker exec** - execute a command
```
docker exec <contatiner_name> <command> <command args>
```
executes a command in docker container
- **Docker run attach and detach**
```
docker run -d <image>
```
runs in detached mode, i.e. container will be running in background.
withoud -d it runs in attached mode where we can see console output of container on our terminal
but can't run commands, we can exit it using Ctrl+C that will also stop the application running in
container and we'll exit the container.
```
docker attach <container_name or container_id>
```
to run a container in attached mode after it was started in detached mode
    

## Run docker containers

## Create a docker image

## Networks in docker

## Docker Compose


## Docker concepts in depth

## Docker Swarm

## Docker vs Kubernetes
