Spring Boot R2DBC Example
An example implementation of Spring Boot R2DBC REST API with PostgreSQL database.

Technology stack
Java 17
Maven
PostgreSQL 16.1
Docker
Java Dependencies
Spring Boot 3.2.1
Spring Data R2DBC
R2DBC PostgreSQL Driver
JUnit 5
Setup
Run postgresql locally (or start from docker-compose file)
Create two databases
postgres (main database)
test (dummy database for integration testing)
Run Spring Boot App
Building Docker Image
Run spring-boot build image plugin
mvn spring-boot:build-image -DskipTests

Run generated docker image
docker run -it -p8080:8080 --network="host" reactive-postgres:0.0.2-SNAPSHOT
