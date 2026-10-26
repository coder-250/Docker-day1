# Docker Day 1 — Fundamentals and First Container

Welcome to Day 1 of the 5-day Docker workshop!

## Learning objectives
- Explain why Docker is useful.
- Distinguish images from containers.
- Run, inspect, stop, start, and remove containers.
- Publish a container port to your computer.

## Prerequisites
Install Docker Desktop (Windows/macOS) or Docker Engine (Linux). Start Docker, then run:
```bash
docker --version
docker info
```

## Repository guide
- `01-concepts/` — core Docker concepts.
- `02-essential-commands/` — commands to practice.
- `03-first-container/` — run Nginx and open it in a browser.
- `04-mini-exercises/` — hands-on tasks.
- `cheat-sheet.md` — quick reference.

## First command
```bash
docker run --rm hello-world
```

## Run a web server
```bash
docker run --name day1-nginx -d -p 8080:80 nginx
```
Open http://localhost:8080.

```bash
docker ps
docker logs day1-nginx
docker stop day1-nginx
docker start day1-nginx
docker rm -f day1-nginx
```

## Troubleshooting
- If Docker cannot connect, start Docker Desktop or the Docker Engine service.
- If port 8080 is busy, use `-p 8081:80` and visit http://localhost:8081.
- If the name already exists, run `docker rm -f day1-nginx` before creating it again.

## Official documentation
- https://docs.docker.com/get-started/
- https://docs.docker.com/reference/cli/docker/container/run/

Day 2 will introduce Dockerfiles and building custom images.
