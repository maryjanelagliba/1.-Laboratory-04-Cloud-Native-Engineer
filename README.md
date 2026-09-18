# 1.-Laboratory-04-Cloud-Native-Engineer


## Mission Overview

In this laboratory, I learned the basic concepts of Docker and containerization. I pulled an official Nginx image from Docker Hub, deployed it as a container, and verified that the web server was working using a local HTTP request. I also practiced managing the container lifecycle by listing, stopping, verifying, and removing a Docker container.

## Objectives

* Learn the basic concepts of Docker containers.
* Pull and use an official Docker image from Docker Hub.
* Deploy an Nginx web server using Docker.
* Map a host port to a container port.
* Verify that a containerized web server is running.
* Practice basic Docker container lifecycle commands.
* Document the Docker deployment process.

## Docker Commands Executed

### Checkpoint 3 - Docker Verification

```bash
docker --version
docker info
systemctl status docker
```

### Checkpoint 4 - Deploy Nginx Container

```bash
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080
```

### Checkpoint 5 - Container Lifecycle

```bash
docker ps
docker stop my-nginx
docker ps
docker ps -a
docker rm my-nginx
```

## Skills Learned

Through this laboratory, I learned how to verify a Docker installation and check the Docker environment. I learned how to download an Nginx image, create and run a container, and connect a host port to a container port. I also learned how to use basic Docker commands to monitor, stop, verify, and remove containers. These skills helped me understand how containers can make application deployment faster and more efficient.

## Challenges Encountered

One challenge I encountered was understanding the difference between a Docker image and a container. I also needed to understand how port mapping works when connecting port 8080 on the host to port 80 inside the Nginx container. Another challenge was remembering the correct commands for stopping and removing a container. By following the commands and observing the terminal output, I was able to successfully complete the Docker deployment and container lifecycle activities.
