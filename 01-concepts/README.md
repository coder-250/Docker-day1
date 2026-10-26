# 01 — Docker concepts

## Why Docker?
Applications may behave differently across laptops, test systems, and servers because their dependencies and configuration differ. Docker packages an application with the environment it needs to help it run consistently.

## Key terms
- **Image:** A template used to create containers.
- **Container:** An isolated process created from an image.
- **Dockerfile:** Instructions for building an image (Day 2).
- **Registry:** A place to store and distribute images, such as Docker Hub.
- **Docker Engine:** The technology that builds and runs containers.
- **Port mapping:** Makes a service inside a container reachable through a host port.
- **Volume:** Keeps data outside a container's writable layer.

## Image vs. container
An image is like a template; a container is an instance created from it. One image can create multiple containers.

## Containers vs. virtual machines
Containers share the host OS kernel and isolate application processes. Virtual machines run a separate guest operating system on virtualized hardware. Each approach has useful roles.

## Check your understanding
1. Can one image create multiple containers?
2. Is a stopped container the same as a deleted container?
3. What is a registry used for?
