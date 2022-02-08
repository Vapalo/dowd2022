FROM openjdk:8

RUN apt update && apt install -y git && \
	git clone https://github.com/docker-hy/material-applications.git ./apps

WORKDIR ./apps/spring-example-project

RUN ./mvnw package

ENTRYPOINT java -jar ./target/docker-example-1.1.3.jar

