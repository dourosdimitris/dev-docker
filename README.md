# README

Ruby On Rails development with Docker.

Based on this [tutorial](https://docs.docker.com/compose/rails/)

## Usage

1. `git clone https://github.com/dourosdimitris/dev-docker.git`
2. `docker-compose run web rails new . --force --no-deps --database=postgresql`
3. add `host: db`, `username: postgres`, `password: password` to `config/database.yml` [more info](https://docs.docker.com/compose/rails/#connect-the-database)
4. create database `docker-compose run web rake db:create`
5. `docker-compose up`

![RoR Welcome Page](https://docs.docker.com/compose/images/rails-welcome.png)

