# README

Ruby On Rails development with Docker.

Based on this [tutorial](https://docs.docker.com/compose/rails/)

## Usage

1. `docker-compose run web rails new . --force --no-deps --database=postgresql`
2. add `host: db`, `username: postgres`, `password: password` to `config/database.yml` [more info](https://docs.docker.com/compose/rails/#connect-the-database)
3. create database `docker-compose run web rake db:create`
4. `docker-compose up`
