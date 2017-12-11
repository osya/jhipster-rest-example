# jHipsterRESTExample

[![Build Status](https://travis-ci.org/osya/jhipster-rest-example.svg?branch=master)](https://travis-ci.org/osya/jhipster-rest-example) [![Coverage Status](https://coveralls.io/repos/github/osya/jhipster-rest-example/badge.svg?branch=master)](https://coveralls.io/github/osya/jhipster-rest-example?branch=master)

This application was generated using JHipster 4.11.1, you can find documentation and help at [http://www.jhipster.tech/documentation-archive/v4.11.1](http://www.jhipster.tech/documentation-archive/v4.11.1).

## Development

To start your application in the dev profile, simply run:

    ./gradlew


For further instructions on how to develop with JHipster, have a look at [Using JHipster in development][].



## Building for production

To optimize the jHipsterRESTExample application for production, run:

    ./gradlew -Pprod clean bootRepackage

To ensure everything worked, run:

    java -jar build/libs/*.war


Refer to [Using JHipster in production][] for more details.

## Testing

To launch your application's tests, run:

    ./gradlew test

For more information, refer to the [Running tests page][].

## Using Docker to simplify development (optional)

You can use Docker to improve your JHipster development experience. A number of docker-compose configuration are available in the [src/main/docker](src/main/docker) folder to launch required third party services.
For example, to start a postgresql database in a docker container, run:

    docker-compose -f src/main/docker/postgresql.yml up -d

To stop it and remove the container, run:

    docker-compose -f src/main/docker/postgresql.yml down

You can also fully dockerize your application and all the services that it depends on.
To achieve this, first build a docker image of your app by running:

    ./gradlew bootRepackage -Pprod buildDocker

Then run:

    docker-compose -f src/main/docker/app.yml up -d

For more information refer to [Using Docker and Docker-Compose][], this page also contains information on the docker-compose sub-generator (`jhipster docker-compose`), which is able to generate docker configurations for one or several JHipster applications.

## Continuous Integration (optional)

To configure CI for your project, run the ci-cd sub-generator (`jhipster ci-cd`), this will let you generate configuration files for a number of Continuous Integration systems. Consult the [Setting up Continuous Integration][] page for more information.

[JHipster Homepage and latest documentation]: http://www.jhipster.tech
[JHipster 4.11.1 archive]: http://www.jhipster.tech/documentation-archive/v4.11.1

[Using JHipster in development]: http://www.jhipster.tech/documentation-archive/v4.11.1/development/
[Using Docker and Docker-Compose]: http://www.jhipster.tech/documentation-archive/v4.11.1/docker-compose
[Using JHipster in production]: http://www.jhipster.tech/documentation-archive/v4.11.1/production/
[Running tests page]: http://www.jhipster.tech/documentation-archive/v4.11.1/running-tests/
[Setting up Continuous Integration]: http://www.jhipster.tech/documentation-archive/v4.11.1/setting-up-ci/


