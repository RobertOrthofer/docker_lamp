# How-To
This is a basic LAMP-Stack in docker-compose, customizable for different needs. It creates containers from two images: Apache + PHP (7.3) and the official MySQL image.

To start , run `docker-compose up` (or `docker-compose up --force-recreate` to rebuild images after a change)

The exposed port of Apache can be configured in `./.env`

Ports and and other configurations are set in the `docker-compose.yml` file.

To enter one of the running docker images and run a command:
```
docker-compose exec <container name> <command name>
```

For instance, this will open a bash shell in the MySQL container:
```
docker-compose exec db bash
```