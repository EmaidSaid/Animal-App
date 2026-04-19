# Animal Image App

This is a Spring Boot application that fetches and stores animal images (cat, dog, bear).

## Run locally
./mvnw spring-boot:run

Open:
http://localhost:8080

## API

POST /api/images/fetch?type=dog&count=2  
GET /api/images/last?type=dog

## Docker

docker build -t animal-image-hub .  
docker run -p 8080:8080 animal-image-hub