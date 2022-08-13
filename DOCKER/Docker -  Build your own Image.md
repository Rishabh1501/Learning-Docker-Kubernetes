Step 1: Make a [[DOCKER/Dockerfile|Dockerfile]]

Step 2: Run the command *docker build <location_of_dockerfile>*
This command will install all the things mentioned in the dockerfile.

Step 3: Check if the image is created using the command *docker image ls*.


> [!NOTE] Naming your Docker image
> Use the build command with the option *-t* to add a name to it.
> **The naming convention:** *<your_name>/<image_name>:<version_of_image>*
> >[!EXAMPLE]
> >*docker build -t rishabhkalra/mymongo:latest .*
> >here *.* is the path of the file





