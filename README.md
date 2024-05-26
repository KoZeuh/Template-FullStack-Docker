<h1 align="center"> Template FullStack Developer Docker </h1>

<p align="center">
This repository contains a Docker Compose template designed to set up a comprehensive development environment for FullStack developers. The environment includes services for PHP with Apache, MariaDB, phpMyAdmin, MongoDB, and a Node.js setup for front-end frameworks like Next.js, Angular, or Vue.js.
</p>

<p align="center">
(It's a way to bypass Wampp, XAMPP, Mamp, etc., and with more services!)
</p>

# Table of Contents

- [Purpose](#purpose)
- [Services & Versions](#services-versions)
- [Build Process](#build-process)
- [Configuration Files](#configuration-files)

# Purpose

This template aims to provide a ready-to-use, isolated development environment that includes all the necessary components for building, testing, and running FullStack applications. By using Docker, you ensure that your development environment is consistent across different setups and systems.

# Services-Versions

- `PHP 8.2 with Apache`: A web server running PHP 8.2 to serve your backend PHP applications.
- `MariaDB (latest)`: A relational database management system for storing your application's data.
- `phpMyAdmin`: A web interface to manage your MariaDB databases.
- `MongoDB (latest)`: A NoSQL database for flexible, JSON-like data storage.
- `Node.js (latest)`: A JavaScript runtime environment for running front-end frameworks such as Next.js, Angular, or Vue.js.


# Build Process

## Clone repository:
```
git clone https://github.com/KoZeuh/Template-FullStack-Docker.git
cd Template-FullStack-Docker
```

## Create a .env file with your environment variables:
```
MYSQL_ROOT_PASSWORD=root_password
MYSQL_DATABASE=my_database
MYSQL_USER=my_user
MYSQL_PASSWORD=my_password

PMA_HOST=db
PMA_PORT=3306
PMA_USER=my_user
PMA_PASSWORD=my_password
```

## Start the services:
`docker-compose up --build`

## Access the services:
```
PHP Application: http://localhost:8080
phpMyAdmin: http://localhost:8081
MongoDB: mongodb://localhost:27017
Node.js Application: http://localhost:3000
```

## Configuration Files

- `php.ini` : Configuration file for PHP settings.
- `www/index.php` : Simple PHP file to verify the PHP server is running.
- `frontend/package.json` : Example configuration for a VueJS application.
- `frontend/src/index.ts` : Example VueJS application entry point.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


