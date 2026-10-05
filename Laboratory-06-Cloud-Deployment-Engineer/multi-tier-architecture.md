# Multi-Tier Architecture

## Two-Tier Architecture

A two-tier architecture separates an application into two main parts: the Web/Application Tier and the Database Tier. In this laboratory, Nextcloud serves as the web application while MariaDB serves as the database.

## Web/Application Tier

The Web/Application Tier is responsible for providing the application's interface to users and handling HTTP requests. In this laboratory, the Nextcloud container provides the web interface that users access through a browser.

## Database Tier

The Database Tier is responsible for storing persistent information used by the application. MariaDB stores information such as user accounts, credentials, and other database information required by Nextcloud.

## Why Separate Them?

Separating the web application and database into different containers makes the system easier to manage and maintain. Each container has a specific responsibility, and the database can be managed separately from the web application.
