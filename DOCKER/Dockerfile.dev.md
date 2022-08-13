# Dockerfile.dev

This is same as [[DOCKER/Dockerfile|Dockerfile]] in every possible way, we use this in development environment to specify it for development needs and not production ready.

Docker **WILL NOT** recognize this file on its own, you will have to explicitly tell Docker that you will use this file for building.

You can specify this information either in the docker build command or inside [[DOCKER/docker-compose.yml|docker-compose.yml]] file.