# Runtrack Job 03 : Docker

```sh
docker search
``` 
We start by using this command to search for the name of the image in Docker Hub like so :

![alt text](images/docker_search.png)

```sh
docker pull
```

We can then pull our image since we now know its exact name .The one we are interested in is on top of the list. 
It gracefully places itself in our file of local and Docker Hub images. 

![alt text](images/pull_and_place.png)

Another method would be to retrieve it by using Docker Desktop search engine. 

![alt text](images/dekstop_image_search.png)

```sh 
docker run
```

Now to run this image we can either use our command with the terminal or do it manually with Docker Desktop.

Exemple with command : 

![alt text](images/run_using_command.png)

Exemple with Docker Desktop built in feature :

First we need to go to our list of images and find the one we want to run. 
Once we find it, click on the "play" icon.

![alt text](images/clicking_icon.png)

This window appears and we apply our wanted optional settings :

![alt text](images/run_window_pop.png)

![alt text](images/optional_settings.png)

Once we are done and click on "run" it should appear in our containers list :

![alt text](images/container_created.png)

To acces the container, we just need to open our browser and use our port as a link : 

![alt text](images/port_link_mario.png)

We can now play super mario on our browser ! 

![alt text](images/mario_game_1.png)

![alt text](images/mario_game_2.png)

![alt text](images/mario_game_3.png)

```sh
docker ps
```

To find our container's ID, we can either use the `docker ps` command : 

![alt text](images/docker_ps_id.png)

Or look at our containers list on Docker Hub : 

![alt text](images/id_container_list.png)

We can use the ID to stop our container :
![alt text](images/stop_container_id.png)

The container with the corresponding ID is stopped. 
It can also be stopped with the stop button to its side directly on the list. 

```sh
docker rm
```

To delete the container completely, we can use the `docker rm` command. 

Either with the container's name or its ID :

![alt text](images/delete_container_1.png)


We can also use Docker Desktop built in method :

![alt text](images/delete_container_2.png)

![alt text](images/delete_container_3.png)

In etiher case, the container no longer exists :

![alt text](images/proof_delete.png)