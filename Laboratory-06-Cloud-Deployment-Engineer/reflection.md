# Mission 6 Reflection

This laboratory helped me understand how Docker Compose can make cloud deployment easier and more organized. Instead of manually typing many Docker commands for every container, I can place the required configuration inside a `docker-compose.yml` file. Once the file is properly configured, Docker Compose can deploy the different services together. This makes the deployment process faster, easier to repeat, and less prone to configuration mistakes.

One important thing I learned is that YAML indentation is very important. YAML uses spaces to organize information, so an indentation mistake or using a Tab instead of spaces can cause the configuration file to become invalid. Docker Compose may not be able to understand the file correctly, which can prevent the application from starting. Because of this, I learned that I need to be careful when creating configuration files.

We also used environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER`. These variables provide the database information required by the Nextcloud application. They also make the configuration easier to understand because the settings are clearly defined inside the Compose file.

Deploying Nextcloud with MariaDB was a good experience because it showed me how a real application can depend on multiple services. Seeing the containers running and accessing Nextcloud through a browser made the concept of multi-container deployment easier to understand.

Since Mission 1, my understanding of Cloud Computing has improved. I now understand that cloud computing is not only about using online services. It also involves infrastructure, containers, networking, storage, automation, and deployment. This mission helped me see how Infrastructure as Code can make cloud environments easier to manage and reproduce.

