# Docker Day 1 Cheat Sheet

| Goal | Command |
|---|---|
| Docker version | `docker --version` |
| Engine details | `docker info` |
| Test installation | `docker run --rm hello-world` |
| Download image | `docker pull nginx` |
| List images | `docker images` |
| Run Nginx | `docker run --name day1-nginx -d -p 8080:80 nginx` |
| Running containers | `docker ps` |
| All containers | `docker ps -a` |
| Read logs | `docker logs day1-nginx` |
| Stop | `docker stop day1-nginx` |
| Start | `docker start day1-nginx` |
| Remove | `docker rm day1-nginx` |
| Force-remove | `docker rm -f day1-nginx` |

Remember: image = template; container = instance. `-p HOST_PORT:CONTAINER_PORT` publishes a port. `docker stop` does not delete a container.
