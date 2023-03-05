# docker-cheat-sheet

### Run docker container 
```
docker container run --publish 3000:80 --detach nginx
```
In the above command `--publish or -p` is used for `port` mapping, `3000` indicates for machine port and `80` indicates for conatiner internal port. `--detach or -d` command is used for the detaching the container, so it can run in the background.
