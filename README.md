# microservices-monorepo  

- This is a spring boot project for microservice architecture with a monorepo.
- available services are
  - api gateway
  - product service
  - order service
  - inventory service
  - notification service

## api-gateway

- An api gateway with keycloak, mysql and docker compose.
- Observabiltiy has been implemented with Grafana stack such as Loki, Tempo, Prometheus.
- The circuit breaker pattern has been implemented with resilience4j.  
- API documentations of other microservices with swagger has been aggregated with in api gateway.

## product-service

- A rest api for product service with mongodb and docker compose.  
- Integration testing with RestAssured and Testcontainer.  
- API documentation with OpenAPI, Swagger and Springdoc openAPI.

## order-service

- A rest api for order service with rest client, mysql and docker compose.
- microservice with event driven architecture  
- kafka with zookeeper, schema registry, avro and kafka ui
- Observabiltiy has been implemented with Grafana stack such as Loki, Tempo, Prometheus.
- Database migration with flyway.  
- Integration test with RestAssured, WireMock and Testcontainer.
- API documentation with OpenAPI, Swagger and Springdoc openAPI.

## inventory-service

- A rest api for inventory service with mysql and docker compose.  
- Database migration with flyway.  
- Integration testing with RestAssured and Testcontainer.
- API documentation with OpenAPI, Swagger and Springdoc openAPI.

## notification-service  

- Notification service with kafka and Java Mail Sender.
- microservice with event driven architecture.
- kafka with zookeeper, schema registry, avro and kafka ui.
- Observabiltiy has been implemented with Grafana stack such as Loki, Tempo, Prometheus.
- Integrate with Mailtrap to send emails.
