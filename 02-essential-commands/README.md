# 02 — Essential Docker commands

## Verify Docker
```bash
docker --version
docker info
docker run --rm hello-world
```

## Images
```bash
docker pull nginx
docker images
docker image inspect nginx
```

## Containers
```bash
docker run -d --name day1-nginx -p 8080:80 nginx
docker ps
docker ps -a
docker logs day1-nginx
docker stop day1-nginx
docker start day1-nginx
docker rm -f day1-nginx
```

## Flags
- `-d`: run in the background.
- `--name`: assign a readable name.
- `-p 8080:80`: map host port 8080 to container port 80.
- `-it`: run with an interactive terminal.
- `--rm`: automatically remove the container when it exits.

`docker ps` lists running containers. `docker ps -a` also lists stopped containers. Stopping a container does not delete it.

## Practice
Run Nginx on port 8081, inspect its logs, stop it, restart it, and remove it.
