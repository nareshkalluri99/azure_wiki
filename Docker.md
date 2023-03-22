Resources:
https://docker-curriculum.com/
https://labs.play-with-docker.com/
https://www.docker.com/products/docker-desktop/

The Docker ecosystem.

**Images** - The blueprints of our application which form the basis of containers. In the demo above, we used the docker pull command to download the busybox image.
**Containers** - Created from Docker images and run the actual application. We create a container using docker run which we did using the busybox image that we downloaded. A list of running containers can be seen using the docker ps command.
**Docker Daemon** - The background service running on the host that manages building, running and distributing Docker containers. The daemon is the process that runs in the operating system which clients talk to.
Docker Client - The command line tool that allows the user to interact with the daemon. More generally, there can be other forms of clients too - such as Kitematic which provide a GUI to the users.
**Docker Hub** - A registry of Docker images. You can think of the registry as a directory of all available Docker images. If required, one can host their own Docker registries and can use them for pulling images.

1. FROM — The base image can be Ubuntu, Redis, MySQL, etc.

2. LABEL — Labeling like EMAIL, AUTHOR, etc.

3. RUN — It is used to tell the container what to do after creating the container from the image. Such as, apk add — update-redis,  rm -fr

Note: If we need to run the file externally that is inside of the container use cp command in the RUN command RUN cp /usr/share/zoneinfo/Asia/Colombo /etc/localtime && echo “Asia/Colombo” > /etc/timezone && apk del tzdata

4. COPY — Copy the files from our host system. src: source path dest: container destination path

5. ADD — It is like a COPY command, but it downloads tar, zip, or web file and extracts and copies inside of our image.

6. WORKDIR — It is used to set the directory that we are going to work. If we are adding some files from host local machine and saves in the container, the working directory path is the default directory

7. ENTRYPOINT — The command the executes inside of container. like server running command in httpd container, bash shell in Ubuntu