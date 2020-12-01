### creating an image

docker build ( image name )

### list all active containers

docker ps -a

### list all containers 

docker ps

### running a container 

docker run  -p 3000:80 ( image name ) (here 3000 is system port and 80 is container's port) 

(attached mode by default)

### runnning a container in dettached mode

docker run  -p 3000:80 -d ( image name )
( dettached mode means the terminal is not listening to the container )

### restart a container from an existing container

docker start ( container name ) ( container runs in the background by default )

( dettached mode by default )

### stop a container 

docker stop ( container name )


### attach to a running container

docker attach (container name | container id)

### fetch past logs by a container 

docker logs (container name | container id)

### Running a container in interactive mode 

<!-- -t because this creates a terminal basically -->

docker run -i -t ( container name )