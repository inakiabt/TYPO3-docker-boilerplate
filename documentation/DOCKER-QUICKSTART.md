[<-- Back to main section](../README.md)

# Docker Quickstart

## Docker short introduction

Create and start containers (eg. first start):

```bash
docker-compose up -d
```

Stop containers

```bash
docker-compose stop
```

Start containers (only stopped containers)

```bash
docker-compose start
```

Build (but not create and start) containers

```bash
docker-compose build --no-cache
```

Delete container content

```bash
docker-compose rm --force
```

Recreate containers (if there is any issue or just to start from a clean build)

```bash
 docker-compose stop
 docker-compose rm --force
 docker-compose build --no-cache
 docker-compose up -d
```

Logs (eg. for debugging)

```bash
# show all logs
docker-compose logs

# ... or only php
docker-compose logs main

# ... or only php and webserver
docker-compose logs main web
```

CLI script (defined in docker-env.yml)

```bash
docker-compose run --rm main cli help
```