# service-spring-boot-docker

Start Docker

$ docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

$ env | grep DOCKER
DOCKER_MACHINE_NAME=default
DOCKER_CERT_PATH=C:\Users\Lucas\.docker\machine\machines\default
DOCKER_TLS_VERIFY=1
DOCKER_HOST=tcp://192.168.99.100:2376
DOCKER_TOOLBOX_INSTALL_PATH=C:\Program Files\Docker Toolbox

$ mvn install dockerfile:build

$ docker run -p 8080:8080 -t springio/spring-boot-docker

$ docker ps
CONTAINER ID        IMAGE                         COMMAND                  CREATED             STATUS              PORTS                    NAMES
bc2a7d2e2e24        springio/spring-boot-docker   "/bin/sh -c 'exec ..."   5 minutes ago       Up 5 minutes        0.0.0.0:8080->8080/tcp   tender_engelbart


