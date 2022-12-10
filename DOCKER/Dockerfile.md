# Dockerfile

This file is used to create a CUSTOM IMAGE, it contains all the configurations required to build your custom image.
The file format of Dockerfile is ***Yaml*** and the file name must be ***Dockerfile*** no change in any spellings.
The Dockerfile is **Case Sensitive**.
***
**STEPS**

**Step 1:** Get a base image for your CUSTOM IMAGE, these are usually operating systems. Use the keyword ***FROM***.
Example: FROM ubuntu

**Step 2:** Install the software's required in the OS installed previously.
Use the command ***RUN*** to run the installation command.
- (Optional) Configure the software if required.
Example: RUN sudo apt update

**Step 3:** For commands. Keyword= ***CMD*** 
***
**KEYWORDS**
- *FROM* : It is used to download a base image.
- *RUN* : It is used to install software and run commands.
- *CMD* : It is used to specify a default command which will run when the container will start.
- *WORKDIR* : Specifies a working directory and if it doesn't exists, it creates them.
- *COPY <current_folder> <destination_folder_inside_container>* : It is used for copying.
- *VOLUMES* : This is used to link volumes between the host and the container, basically it links the folders together and help in syncing the files between the container and the host machine folder.
- *EXPOSE <port_number>* : This is used to expose a port.
- *ENTRYPOINT ["Executable Command"]* : This is similar to CMD but in this we just specify the default command name, such as sleep and pass the argument when we run the container like *docker run <image_name> 50*, here the sleep command will take the argument 50 and sleep for 50 seconds.

***
> [!EXAMPLE] Dockerfile  
> Check Practical Folder

