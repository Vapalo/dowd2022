FROM openjdk:18-alpine

RUN apk add --no-cache git && \
		git clone https://github.com/Vapalo/Spring-boot-project.git /app
	
WORKDIR /app

RUN chmod +x mvnw && ./mvnw package

ENTRYPOINT java -jar /app/target/AlbumList-0.0.1-SNAPSHOT.jar
