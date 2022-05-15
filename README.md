### Docker

### Image

- actual package (eg. config, postgresSQL v9.3, start script)

### Container

- Running environment for image
- Layers of images
- Linux base image (eq. alpine:3.10)
- Application image on top (eg. postgres:10.10)

### Basic commands

1. Start a container: run
2. List running containers: ps
3. List all containers: ps-a
4. Stop a running container: stop {name/id}
5. Remove a container: rm {name/id}
6. List images: images
7. Remove image: rmi {image}
8. Pull: docker pull {image}
9. Execute a command: docker exec {container} cat /etc/hosts
10. Run - attach & detach: docker run -d {image} , docket attach image

### Run

1. Run in interactive mode (input etc.): docker run -i {image}
2. Psuedo terminal (prompt etc): docker run -it {image}
3. Port mapping: docker run -p {host_port}:{container_port} {image}
4. Volume mapping: docker run -v /opt/datadir:/var/lib/mysql mysql
5. Env variable: docker run -e {APP_COLOR=blue} {image}

### Debugging

1. Inspect container: docker inspect {name/id}
2. Container logs: docker logs {name/id}
3. Inspect env variable: docker inspect {image}
