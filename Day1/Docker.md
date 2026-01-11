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

### Stop the container
```docker
docker stop container_name
```

### To see the list of images
```docker
docker images
```

### To remove images
```docker
docker rmi nginx
```

### Pull the image from Docker Hub
```docker
docker pull nginx
```

### To run the image for 15 seconds
```docker
docker run ubuntu sleep 15
```

### execute the command
```docker
docker exec container_id cat /etc/*release*
```

### 
docker run port -d(run in background) --name 
docker run -p 8080:3036 -d --name webapp ubuntu

Run - attach and detach

docker run -d /opt/webapp - run in the background

docker attach a043d(id)

### Volume mapping
docker run -v /opt/datadir:/var/lib/mysql mysql

### Inspect Container
```
docker inspect ubuntu
```
### Container Logs
```
docker logs name/container_id
```

### To run with version
```
docker run ubuntu:17.0
```

Demo
```
docker run timer -d
docker attach containerid
```


























