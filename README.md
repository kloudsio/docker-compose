# docker-compose in a container

Docker Compose in an Alpine Linux based container. Only 30MB in size!  
Suitable for running inside boot2docker.
 
```
$ docker run --rm -it \
-v $(pwd):$(pwd) -v /var/run/docker.sock:/var/run/docker.sock \
-e COMPOSE_PROJECT_NAME=$(basename $(pwd)) -w="$(pwd)" \
blinkreaction/docker-compose
```
