# Runtrack jour 01 : Docker

```sh
docker version
```
This command allows us to check which version of docker we're using.


![alt text](<images_docker/Capture d'écran 2025-02-11 100408.png>)


```sh
docker info
```
Displays system wide information regarding the Docker installation 

![alt text](<images_docker/Capture d'écran 2025-02-11 100850.png>)

```sh
docker ps
```
Provides a list of containers on your machine as well as their specific state (running or not, size..)

![alt text](<images_docker/Capture d'écran 2025-02-11 101642.png>)

```sh
docker images
```
Displays a list of the images you pulled and their satuts.

![alt text](<images_docker/Capture d'écran 2025-02-11 102225.png>)

```sh
docker run
```

Starts a new container and executes a command inside it, it pulls an image if needed. 

![alt text](<images_docker/Capture d'écran 2025-02-11 102523.png>)

```sh
docker stop
```
Stops one or more running containers.

![alt text](<images_docker/Capture d'écran 2025-02-11 103429.png>)

```sh
docker pull
```
The "docker pull" command downloads a Docker image locally on the host from a public or private registry. Here we pulled nginx's latest image version using the ":latest" option.

![alt text](<images_docker/Capture d'écran 2025-02-11 105748.png>)

```sh
docker images
```
As said previously, this command displays all of your images. Since we pulled nginx's image, we can see where it's saved locally, which version we're using, its ID, when it was created and how much space it takes. 

![alt text](<images_docker/Capture d'écran 2025-02-11 105955.png>)

```sh
docker run <image_name>
```

Using docker run to create container for nginx's image. `-it`option allows to run the container interacively. `-i` for interactive mode and `-t` for accessing terminal. This can be useful if the image you're running is an OS for exemple.

  ```--rm``` option makes it so this container will be deleted if stopped. 

  `-p` is used to assign a port for your image.

![alt text](<images_docker/Capture d'écran 2025-02-11 110716.png>)

```sh
Access container using an explorer
``` 
To acces your container using an exploreur, we use the port we assigned it as an url in the search tab.

![alt text](<images_docker/Capture d'écran 2025-02-11 114853.png>)

![alt text](<images_docker/Capture d'écran 2025-02-11 114619.png>)