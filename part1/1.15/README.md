# Dockerfile for spring boot project

This dockerizes my [spring boot project](https://github.com/Vapalo/Spring-boot-project).

The dockerfile is hosted at [vapalo/spring-boot-project](https://hub.docker.com/r/vapalo/spring-boot-project).

## Steps to run

```bash
$ docker pull vapalo/spring-boot-project

$ docker run --rm -p 8080:8080 vapalo/spring-boot-project
```

* --rm -> Removes the container once it stops
* -p 8080:8080 -> Ports to be exposed. On the left side is the host port and on the left the containers port
* vapalo/spring-boot-project -> name of the container

You also could add the `-d` option to detach the container from your terminal so it runs in the background.

## It's running. What do?

Once the container is running navigate to `localhost:8080` and use one of the following credentials:

| Username | Password      |
| ---      | ---           |
| user     | salasana      |
| admin    | adminsalasana |

Admin account can perform full crud functionalities and user has read access only
