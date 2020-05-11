# Heroku Gunicorn boilerplate [![Django CI](https://github.com/scoutbee/heroku-gunicorn-boilerplate/workflows/Django%20CI/badge.svg)](https://github.com/scoutbee/heroku-gunicorn-boilerplate/actions)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/scoutbee/heroku-docker-gunicorn-boilerplate)

This boilerplate provides an example of a React / Django (Client / Server) based application hosted on Heroku with a Gunicorn Django setup.

## Relevant files

### [.buildpacks](https://github.com/scoutbee/heroku-gunicorn-boilerplate/blob/master/.buildpacks)

The `.buildpacks` file is used to use multiple Heroku buildpacks for different sub directories.

Find more about that file in the [Buildpack documentation](https://github.com/negativetwelve/heroku-buildpack-subdir).

### [app.json](https://github.com/scoutbee/heroku-gunicorn-boilerplate/blob/master/heroku.yml)

The app.json file is there for specifiying all the dependencies of your Heroku application. These can be addon-specific ones (Postgres e.g.), environment variables which needs to be set or hardware specification for you dynamic created environments via Review Apps.

Find more about that file in the [Heroku docs](https://devcenter.heroku.com/articles/app-json-schema).

### [Procfile](https://github.com/scoutbee/heroku-gunicorn-boilerplate/blob/master/Procfile)

Via this file you instruct Heroku which processes should be run on the Dynos (containers). Also you can set there a command which will be execute on each release to run e.g. SQL migrations.

Find more about that file in the [Heroku docs](https://devcenter.heroku.com/articles/procfile).

## Other boilerplates for React / Django

- [Heroku Docker Gunicorn](https://github.com/scoutbee/heroku-docker-gunicorn-boilerplate)
- [Heroku NGINX Gunicorn](https://github.com/scoutbee/heroku-nginx-gunicorn-boilerplate)
