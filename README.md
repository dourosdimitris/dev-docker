
# README

Ruby On Rails development with Docker.

Based on this [tutorial](https://docs.docker.com/compose/rails/)


## Usage

1.  `git clone https://github.com/dourosdimitris/dev-docker.git`

2.  `cd dev-docker`

3.  create app (see `rails new --help` for more info)
	a.	full stack: `docker-compose run web rails new . --force --no-deps --database=postgresql`
	b. api only: `docker-compose run web rails new . --api --skip-spring -C -T --force --no-deps --database=postgresql`

4. add `host: db`, `username: postgres`, `password: password` to `config/database.yml`  [more info](https://docs.docker.com/compose/rails/#connect-the-database)

5. `docker-compose build`

6. create database `docker-compose run web rake db:create`

7.  `docker-compose up`


![RoR Welcome Page](https://docs.docker.com/compose/images/rails-welcome.png)