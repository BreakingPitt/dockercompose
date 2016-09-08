[![Build Status](https://travis-ci.org/BreakingPitt/dockercompose.svg?branch=master)](https://travis-ci.org/BreakingPitt/dockercompose)
[![Coverage Status](https://coveralls.io/repos/github/BreakingPitt/dockercompose/badge.svg?branch=master)](https://coveralls.io/github/BreakingPitt/dockercompose?branch=master)

Docker Compose repository.
================================

Docker Compose is a Docker tools that allow us describe the relationship between the containers in our multi-container application.

Applications based on micro-services can use multiple containers to provide a service, for example, one can contain a PostgreSQL database, other a key/value database like REDIS or a search tool like ElasticSearchfor document searching.

If our application have multiple Docker containers using the **docker run** command with each container can make us feel uncomfortable. In this point Docker Compose tool allow us define our multi-container application in a file with the same properties that would point to the **docker run** command.

Docker Compose projects.
------------------------
* Jenkins.
* Jenkins 2.
* MySQL (No_data_container).
* MySQL (With_data_container).
* PostgreSQL (No_data_container).
* PostgreSQL (With_data_container).
* Service Discovery.

How to run Docker Compose projects.
-----------------------------------

To start a Docker Compose project, inside the project directory run the following command:

**cd jenkins && docker-compose run -d**

The flag *-d* runs the containers in daemon mode.

To stop a Docker Compose project, inside the project directory run the following command:

**cd jenkins && docker-compose stop && docker-compose rm -v**

To remove the volumes used by our containers, inside the project directory run the following command:

**cd jenkins && docker-compose rm -fv**
