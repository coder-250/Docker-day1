# 04 — Day 1 mini-exercises

## Exercise 1: Installation
1. Display the Docker version.
2. Check that the Docker Engine is reachable.
3. Run `hello-world`.

## Exercise 2: Images and containers
1. Pull the Nginx image.
2. List local images.
3. Start two Nginx containers with different names and host ports.
4. Visit both in a browser. Hint: use `8080:80` and `8081:80`.

## Exercise 3: Inspect and clean up
1. List running containers.
2. Read one container's logs.
3. Stop it.
4. Find it using `docker ps -a`.
5. Remove your practice containers.

## Reflection
1. What is the difference between `docker stop` and `docker rm`?
2. What does `-d` do?
3. Why are host and container ports different?
4. What does `--rm` do?

## Success checklist
- [ ] Docker commands work on my machine.
- [ ] I can explain image vs. container.
- [ ] I can run Nginx in a browser.
- [ ] I can inspect, stop, restart, and remove a container.
