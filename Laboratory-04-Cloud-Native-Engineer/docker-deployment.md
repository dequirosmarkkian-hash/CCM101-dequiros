# Docker Deployment

## Docker Commands Executed

### 1. Check Docker Version

```bash
docker --version
```

This command displays the installed Docker version and verifies that Docker is available in the terminal.

### 2. Check Docker Status and Information

```bash
docker info
```

This command displays information about the Docker environment, including the server, containers, images, and storage configuration.

### 3. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub so that it can be used to create a container.

### 4. Run the Nginx Container

```bash
docker run -d -p 8080:80 --name nginx-server nginx
```

This command creates and starts an Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### 5. Test the Nginx Web Server

```bash
curl http://localhost:8080
```

This command sends a local HTTP request to the Nginx server and verifies that the web server is responding.

## Container Lifecycle

### 6. List Running Containers

```bash
docker ps
```

This command lists the containers that are currently running.

### 7. Stop the Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container.

### 8. Verify the Container Is Stopped

```bash
docker ps -a
```

This command lists all containers, including stopped containers, allowing the user to verify that the Nginx container is no longer running.

### 9. Remove the Container

```bash
docker rm nginx-server
```

This command permanently removes the stopped Nginx container from the Docker environment.

## Screenshots

* `docker-version.png` – Docker installation and environment verification.
* `nginx-running.png` – Successful Nginx HTTP response.
* `container-lifecycle.png` – Container listing, stopping, verification, and removal.
