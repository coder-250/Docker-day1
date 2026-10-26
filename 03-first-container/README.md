# 03 — Your first container

We will run Nginx, a web server, using an image available on Docker Hub.

## 1. Run Nginx
```bash
docker run --name day1-nginx -d -p 8080:80 nginx
```

If the name already exists:
```bash
docker rm -f day1-nginx
```
Then run the first command again.

## 2. Open it
Visit http://localhost:8080. You should see the Nginx welcome page.

## 3. Inspect
```bash
docker ps
docker logs day1-nginx
docker port day1-nginx
```

## 4. Stop and restart
```bash
docker stop day1-nginx
docker ps -a
docker start day1-nginx
```

## 5. Clean up
```bash
docker rm -f day1-nginx
```

In `-p 8080:80`, `8080` is the port on your computer and `80` is the port inside the container. If 8080 is occupied, use `-p 8081:80`.
