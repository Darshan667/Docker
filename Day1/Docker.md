# Docker
# What is Docker ?
Docker is a containerization platform that provides an easy way to containerise your application, which means using Docker you can build container images, run the
images to create containers and also push these containers to container registries such as Docker Hub



Docker has 2 editions 
1. Community Edition
2. Enterprise Edition


### Run- start a container
```docker
docker run nginx
```

### To list the containers
```docker
docker ps 
docker ps -a
```

docker stop container_name

docker images - to see the list of images

docker rmi nginx - remove the image 

docker pull nginx - download the image

docker run ubuntu

docker run ubuntu sleep s

docker exec distracted_file cat /etc/hosts

Run - attach and detach

docker run -d /opt/webapp - run in the background

docker attach a043d(id)























