# Docker and Docker Compose commands

## Build

- Build services

  ```sh
  docker-compose build
  ```

## Containers

- Startup services

  ```sh
  docker-compose up
  ```

- Startup service

  ```sh
  docker-compose up <service>
  ```

- Run command into service

  ```sh
  docker-compose exec <service> <command>
  ```

- List active containers

  ```sh
  docker container ls
  ```

  or

  ```sh
  docker ps
  ```

- List all containers

  ```sh
  docker container ls -a
  ```

  or

  ```sh
  docker ps -a
  ```

- Stop active container

  ```sh
  docker container stop <container_name>
  ```

  or

  ```sh
  docker stop <container_name>
  ```

- Start container

  ```sh
  docker container start <container_name>
  ```

  or

  ```sh
  docker start <container_name>
  ```

- Stop active services

  ```sh
  docker-compose stop
  ```

- Stop active service

  ```sh
  docker-compose stop <service>
  ```

- Remove active services

  ```sh
  docker-compose down
  ```

- Remove container

  ```sh
  docker container rm <container_name>
  ```

  or

  ```sh
  docker rm <container_name>
  ```

- Remove container with force

  ```sh
  docker container rm <container_name> -f
  ```

  or

  ```sh
  docker rm <container_name> -f
  ```

- Prune containers

  ```sh
  docker container prune
  ```

- Prune containers with force

  ```sh
  docker container prune -f
  ```

## Images

- List images

  ```sh
  docker image ls
  ```

- Remove image

  ```sh
  docker image rm <image_id>
  ```

- Remove image with force

  ```sh
  docker image rm <image_id> -f
  ```

- Prune images

  ```sh
  docker image prune
  ```

- Prune images with force

  ```sh
  docker image prune -f
  ```

## Volumes

- List volumes

  ```sh
  docker volume ls
  ```

- Remove volume

  ```sh
  docker volume rm <volume_name>
  ```

- Prune volumes

  ```sh
  docker volume prune
  ```

- Prune volumes with force

  ```sh
  docker volume prune -f
  ```

## Networks

- List networks

  ```sh
  docker network ls
  ```

## Actions

- Execute command into container

  ```sh
  docker exec -it <container_name> <command>
  ```

  Example:

  - Enter the container:

    ```sh
    docker exec -it <container_name> bash
    ```

- View container logs

  ```sh
  docker logs <container_name>
  ```

- View container logs with real time

  ```sh
  docker logs <container_name> -f
  ```
