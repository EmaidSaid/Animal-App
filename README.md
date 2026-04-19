# Animal Image App

This project is a small Spring Boot application built for the TAM technical challenge.
It provides:
- a REST endpoint to fetch and store animal images by type and count
- a REST endpoint to retrieve the last stored image for a given animal type
- a simple HTML page to interact with the service from the browser
## Supported animal types
- cat
- dog
- bear
## Tech stack
- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database
- Maven
- Docker

## Database
The application uses H2 as an embedded in-memory database, so no external database setup is required.

## Run locally
```bash
./mvnw spring-boot:run

## Open:
http://localhost:8080

## API

POST /api/images/fetch?type=dog&count=2  
GET /api/images/last?type=dog

## Docker

docker build -t animal-image-hub .  
docker run -p 8080:8080 animal-image-hub
