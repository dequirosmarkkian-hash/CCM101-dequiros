# Mission Reflection

This laboratory activity helped me understand the practical difference between Virtual Machines and containers. A Virtual Machine requires a complete operating system to be installed and started before applications can run. Because of this, the boot process can take several minutes and requires more system resources. In comparison, a Docker container uses the host operating system's kernel, so it can start much faster and requires fewer resources. This makes containers useful for applications that need to be deployed quickly and efficiently.

The port mapping `-p 8080:80` is necessary because the Nginx web server runs on port 80 inside the container, while port 8080 is used on the host to access the application. The mapping connects the host's port 8080 to the container's port 80. Without this mapping, the Nginx service inside the container would not be directly accessible through the host's port 8080.

When the `docker rm` command is used, the specified stopped container is removed from Docker. The container itself and its writable container layer are deleted. However, the Docker image used to create the container remains available unless it is separately removed. This shows the difference between a container and an image.

Containerization also changes how developers and IT operations teams work together. Developers can package an application together with its dependencies, while operations teams can deploy the same containerized application in different environments. This supports DevOps practices by making deployment more consistent and repeatable.

My GitHub portfolio is evolving from simple cloud research into a more practical technical portfolio. Laboratory 4 adds Docker, containerization, Linux terminal experience, deployment, and technical documentation. The screenshots and Markdown files provide evidence of the skills I practiced during the laboratory activity.
