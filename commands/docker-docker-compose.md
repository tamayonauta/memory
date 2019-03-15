# Docker and Docker Compose commands

## Build

### Build services

```sh
docker-compose build
```

## Containers

### Startup services

```sh
docker-compose up
```

### Startup service

```sh
docker-compose up <service>
```

### Run command into service

```sh
docker-compose exec <service> <command>
```

### List active containers

```sh
docker container ls
```

### List containers

```sh
docker container ls -a
```

### Stop active services

```sh
docker-compose stop
```

### Stop active service

```sh
docker-compose stop <service>
```

### Remove active services

```sh
docker-compose down
```

### Remove container

```sh
docker container rm <container_id>
```

### Remove container with force

```sh
docker container rm <container_id> -f
```

## Images

### List images

```sh
docker image ls
```

### Remove image

```sh
docker image rm <image_id>
```

### Prune images

```sh
docker image prune
```

### Prune images with force

```sh
docker image prune -f
```

## Volumes

### List volumes

```sh
docker volume ls
```

### Remove volume

```sh
docker volume rm <volume_name>
```

### Prune volumes

```sh
docker volume prune
```

### Prune volumes with force

```sh
docker volume prune -f
```