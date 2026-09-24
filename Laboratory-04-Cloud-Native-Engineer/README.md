# Laboratory-04-Cloud-Native-Engineer


## Mission Overview

This laboratory activity focuses on cloud-native technologies, particularly Docker containers. The activity demonstrates the differences between traditional Virtual Machines and containers and provides practical experience using Docker to deploy an Nginx web server.

## Objectives

* Differentiate between Virtual Machines and Containers.
* Access a Docker-enabled cloud environment using KillerCoda.
* Execute basic Docker CLI commands.
* Pull and run an Nginx container.
* Map a host port to a container port.
* Manage the lifecycle of a Docker container.
* Document container operations using Markdown.

## Docker Commands Executed

```bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name nginx-server nginx
curl http://localhost:8080
docker ps
docker stop nginx-server
docker ps -a
docker rm nginx-server
```

## Skills Learned

Through this laboratory activity, I learned how containers differ from traditional virtual machines and how Docker can be used to package and run applications. I also learned basic Docker commands for downloading images, creating containers, checking running containers, stopping containers, and removing containers. I gained practical experience deploying an Nginx web server and mapping a host port to a container port.

## Challenges Encountered

One challenge was becoming familiar with Docker commands and understanding the difference between an image and a container. Another challenge was understanding port mapping and how the host port connects to the web server running inside the container. Using the KillerCoda environment helped me practice these commands in a Linux-based cloud environment.

