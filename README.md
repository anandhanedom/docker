### Docker

### Image

- actual package (eg. config, postgresSQL v9.3, start script)
- movable

### Container

- Running environment for image
- Layers of images
- Linux base image (eq. alpine:3.10)
- Application image on top (eg. postgres:10.10)

### Basic commands

1. List running containers: docker ps
2. Run container in detached mode: docker run -d redis
3. Stop a container: docker stop {container_id}
4. Start a container: docker start {container_id}
5. List running and stopped containers: docker ps -a
6. Pull image and start container: docker run redis
7. Bind host port to container port: docker run -p{host_port}:{container_port} redis:4.0
8. List docker images: docker images
9. Run container with a custom name: docker run -d -p6001:6379 --name redis-older redis:4.0

### Debugging commands

1. Show logs: docker logs {container_id / name}
2. Navigate inside container(envs, config etc - virtual file system) : docker exec -it {container_id/container_name} /bin/bash
 
