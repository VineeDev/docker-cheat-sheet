# docker-cheat-sheet

### Run docker container 
```
docker container run --publish 3000:80 --detach nginx
```
In the above command `--publish or -p` is used for `port` mapping, `3000` indicates for machine port and `80` indicates for conatiner internal port. `--detach or -d` command is used for the detaching the container, so it can run in the background.

### To see the processes running inside the docker container 
```
docker top nginx
```
it will list out the all processes running inside the container.

### Inspect a container
```
docker inspect container 
```
### Performance stats of all containers
```
docker stats containers
```

### Docker network concepts 

#### Container port
``` docker container port conatiner
80/tcp -> 0.0.0.0:80
```
#### Container IPAddress
``` 
docker container inspect --format '{{.NetworkSettings.IPAddress}}' container
```
