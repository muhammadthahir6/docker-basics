# Docker basic commands

```bash
# Show the Docker version information

docker version

# run a docker image

docker run <image name>

docker run hello-world

# run a docker image with tag

docker run <image name>:tag

docker run node:16-alpine

# interactive mode

docker run it <image name>

docker run -it node:16-alpine

# docker detached mode

docker run -d <image name>

# get logs of a container

docker logs <container id>

# docker processes

docker ps 

# docker running containers

docker container ls

# stop a running container 

docker stop <container ID>

# remove a container

docker container rm 2fefb4099f67

# locally list available images

docker image ls

# remove an image

docker image rm <image>:<tag>

# get information on Docker objects

docker inspect <instance id>

# docker expose port 

docker run -p 5009:27017 mongo

```