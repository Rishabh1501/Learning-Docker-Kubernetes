# DOCKER COMMANDS
***
***
>[!Important] COMMAND TO CHECK DATA USAGE BY EACH FILE
>`docker run --rm imagename du -k /`
***
- *docker ps*
This command is used to see the running containers.
OPTIONS-
- -a or --all: This is used to list all the containers present not just running ones.
***
- *docker run <image_name>*
This command is used to run an image and creates a new container every time it is executed.
If the image is not present in the machine, it will extract the image from the docker hub, install it and then run it in a container.

Docker run command consists of two commands 
- docker create: It creates an Image.
- docker start: It starts an Image.

OPTIONS-
- -i : interactive mode, allows you to use your keyboard inside the container
- -t : creates a pseudo terminal.
- -it: its just -i and -t together, use it for easy termination of docker run command by pressing Ctrl+C .
- -p : used to create port to port connections between container and the host. USAGE: *-p <host_port> : <container_port>*
- -d : detaches the container from the terminal.
- -v : Attaches volume, used to map files between docker and host, in simple terms you don't have to run the build command every time you make a change. USAGE: *-v <location_in_host_machine> : <location_inside_container>*
- -e : It is used to attach environment variables. USAGE: *-e <env_name>*
- --env-file : It is used to provide the path of the env file in which all of your environment variables are present.
***
- *docker pull <image_name>*
This command is used to pull and image from the docker hub.
***
- *docker stop <container_id>*
This command is used to stop a container and put it into **exited** state.
To start image again, use *docker start*

This is the **Recommended** command for stopping a docker container, as it closes down the processes in the way they are meant to be stopped, rather than just killing them, in simple terms it shuts it down rather than pulling the plug.
***
- *docker kill <containter_id>*
This command kills the container, basically stopping it like pulling the plug.
**Not recommended** to use, use *docker stop* instead.
***
- *docker pause*
This command is used to stop a container and put it into **paused** state.
To get it into started mode, use command *docker unpause*
***
- *docker start <container_id>*
This will start a container with it's container id.

OPTIONS:
- -a: This executes the default command for the image or in some cases where there is no default command, it executes last used command.
***
- *docker system prune*  (**WARNING**)
This command will delete all the images and the containers present.
***
- *docker exec <container_id>*
It is used to run a command in a **Running** container.

OPTIONS:
- -i: interactive mode
- -t: Terminal mode
***
- *docker image <command_use>*
This command is used for all image related stuff, just type *docker image* inside the terminal and see the list of commands.
Examples:
- *docker image ls* : Displays all the images present/installed.
- *docker image rm <image_name>* : Used to delete/remove an image from the system.
***
- *docker build <path_of_dockerfile>*
This command is used to build a custom image using the [[DOCKER/Dockerfile|Dockerfile]].
OPTIONS:
- -t : use it to name your image.
- -f : It can be used to specify a different file location whose name is not Dockerfile, but consists of all the same contents as Dockerfile. 
***
- *docker compose up*
This command is used to build an image using the [[DOCKER/docker-compose.yml|docker-compose.yml]] file.
It does not build the image unless the option --build is specified explicitly.
OPTIONS:
- --build: use this to build the image.
***
- *docker compose*
This command is used access all the features related to [[DOCKER/docker-compose.yml|docker-compose.yml]] file, containers and images.
OPTIONS:
- ps: used to see the running docker-compose containers, but can only be executed on terminal when the [[DOCKER/docker-compose.yml|docker-compose.yml]] file is present in the current working directory.
***

















