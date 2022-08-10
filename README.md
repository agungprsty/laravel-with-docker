# Laravel with Docker 🐳

<p align="center">
    <img src="https://digitalwiki.info/storage/uploads/images/Lm3lcerkhX29YvXuR1EO8gDOeEUX4iy3mO3HIVDG.png" alt="docker-laravel">
</p>

## Introduction

Build a simple laravel application development environment with docker-compose.


## Requirement
- Docker ^19.*

## Usage

1. Click [Use this template](https://github.com/agungprsty/laravel-with-docker/generate)
2. Git clone & change directory
3. Execute the following command

```bash
$ make create-project # Install the latest Laravel project
```

## Show Application
http://localhost

## Container details

### app container

- Base image
  - [php](https://hub.docker.com/_/php):8.1-fpm
  - [composer](https://hub.docker.com/_/composer):2.3
  - [npm](https://deb.nodesource.com/setup_lts.x):latest

### web container

- Base image
  - [nginx](https://hub.docker.com/_/nginx):stable-alpine

### db container

- Base image
  - [mysql](https://hub.docker.com/_/mysql):8.0

### phpmyadmin container

- Base image
  - [phpmyadmin](https://hub.docker.com/_/phpmyadmin):latest

### redis container

- Base image
  - [redis](https://hub.docker.com/_/redis):latest

### rabbitmq container

- Base image
  - [rabbitmq](https://hub.docker.com/_/rabbitmq):latest

## Thanks and Inspired by:
> [@ucan-lab](https://github.com/ucan-lab)