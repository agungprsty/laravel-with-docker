# Laravel with Docker 🐳

<p align="center">
    <img src="./docker/images/laravel+docker.png" alt="docker+laravel">
</p>

## Introduction

Build a simple laravel application development environment with docker-compose.


## Requirement
- Docker ^19.*

## Installation

1. click [Use this template](https://github.com/agungprsty/laravel-with-docker/generate)
2. git clone & change directory
3. execute the following command

```bash
$ make create-project # Install the latest Laravel project
```
4. set src/.env variable :
```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=admin
DB_PASSWORD=admin
```
5. show application in [http://localhost](http://localhost)
6. show phpmyadmin in [http://localhost:81](http://localhost:81)
7. list execute command in [Makefile](Makefile).

## Container details :
- ``app`` use image:
  - [php](https://hub.docker.com/_/php):8.1-fpm
  - [composer](https://hub.docker.com/_/composer):2.3
  - [npm](https://deb.nodesource.com/setup_lts.x):latest
- ``web`` use image:
  - [nginx](https://hub.docker.com/_/nginx):stable-alpine
- ``db`` use image:
  - [mysql](https://hub.docker.com/_/mysql):8.0
- ``phpmyadmin`` use image:
  - [phpmyadmin](https://hub.docker.com/_/phpmyadmin):latest

> Optional
> - ``redis`` use image:
>   - [redis](https://hub.docker.com/_/redis):latest
> - ``rabbitmq`` use image:
>   - [rabbitmq](https://hub.docker.com/_/rabbitmq):latest

## Thanks and Inspired by:
> [@ucan-lab](https://github.com/ucan-lab)