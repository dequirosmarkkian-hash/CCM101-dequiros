# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block defines the containers that will be created and managed by Docker Compose. In this laboratory, it contains two services: `database` for MariaDB and `app` for Nextcloud.

## How Does Nextcloud Find the Database?

Nextcloud finds the MariaDB container through the `MYSQL_HOST` environment variable.

The configuration uses:

```yaml
- MYSQL_HOST=database
```

The value `database` refers to the database service defined in the Docker Compose file. This allows the Nextcloud application container to communicate with the MariaDB container.

## `docker run` vs. `docker-compose up -d`

`docker run` is normally used to create and start an individual container using a command with its required settings.

`docker-compose up -d` uses the configuration written in the `docker-compose.yml` file to create and start multiple related containers together. The `-d` option runs the containers in the background.

## Infrastructure as Code

The Docker Compose file acts as Infrastructure as Code because the infrastructure configuration is written in a YAML file. Instead of manually entering every configuration command, the same configuration can be used to deploy the application stack consistently.
