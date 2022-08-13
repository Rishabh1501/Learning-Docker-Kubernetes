# docker-compose.yml

This file is used to link various services together, all the services mentioned inside this file automatically becomes connected to each other.
**Tabs** are very important in this file like python.
The file format is **yaml**.

> [!IMPORTANT] Another use
> This file is **NOT** just used for linking various services together but it is also used when the docker run command becomes very big.
> Such as ports or volumes.

**LAYOUT**

- **Version** on top, it tells us about the version of the docker-compose to use. *version: "<version_number>"* (version 3 is the latest)

- **Services** contain the information about the images, such as image name, custom build, ports etc.


> [!NOTE] Learn More
> Refer to the [Documentation](https://docs.docker.com) for more in-depth details also look at the Examples folder for examples.

