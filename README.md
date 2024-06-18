# Microservices Project README

Welcome to the Microservices Project README! This document provides an overview of the project's topics, steps taken, and key concepts.

## Topics Covered

1. [Service Discovery](#service-discovery)
2. [Centralised Configuration](#centralised-configuration)
3. [Distributed Tracing](#distributed-tracing)
4. [Event Driven Architecture](#event-driven-architecture)
5. [Centralised Logging](#centralised-logging)
6. [Circuit Breaker](#circuit-breaker)
7. [Secure Microservice using KeyCloak](#secure-microservice-using-keycloak)

## Project Overview

This project focuses on building a microservices architecture using Spring Cloud. The architecture involves several services, each addressing specific functionalities. Here's an overview of the steps taken for each service:

### Step 1 - Product Service

- Created the Product service with initialized endpoints.
- Tested the endpoints using Postman.
- Implemented automated tests using the "testContainers" library for integrated testing.
- Utilized Docker containers for simulating dependencies, such as MongoDB.
- Emphasized integrated tests over unit tests for the entire application context.
- Leveraged test containers for MongoDB and Jupiter/Junit5 for test generation.

### Step 2 - Order Service

- Developed the Order service, utilizing MySQL as the order database.
- Demonstrated the reuse of the Spring application for different services.

### Step 3 - Inventory Service

- Created the Inventory service, showcasing the expansion of the microservices ecosystem.

### Step 4 - Notification Service

- Initiated the Notification service.
- Established synchronous and asynchronous communication among Notification, Order, and Inventory services.

### Step 5 - Inter-Process Communication

- Explored synchronous and asynchronous communication.
- Utilized WebClient from Spring WebFlux for HTTP client communication.
- Added WebClient dependency to the root .pom file.

### Step 6 - Service Discovery

- Set up Spring Cloud Netflix Eureka Server for service discovery.
- Configured client-side load balancing using Eureka client library.
- Performed disruptive tests to validate service availability even with a downed discovery server.

### Step 7 - API Gateway

- Utilized Spring Cloud Gateway as the API Gateway.
- Defined routes to services in the API Gateway module's application.properties.
- Registered the API Gateway service as a client with the discovery server.

### Step 8 - Secure Microservices using KeyCloak

- Set up KeyCloak authentication and authorization server.
- Configured KeyCloak to enable secure communication with the API Gateway.

### Step 9 - Implementing Circuit Breakers

- Implemented circuit breakers using Resilience4J library.
- Enabled Actuator for monitoring health metrics.
- Annotated controller methods with circuit breaker and fallback logic.
- Explored fault tolerance features like timeouts and retry mechanisms.

### Step 10 - Distributed Tracing

- Implemented distributed tracing using Spring Cloud Sleuth.
- Utilized Trace IDs and Span IDs for tracking requests.
- Visualized traces using Zipkin.

### Step 11 - Event Driven Architecture using Kafka

- Utilized Spring for Apache Kafka for event-driven architecture.
- Set up Kafka using Docker for local development.
- Created Kafka clusters with Zookeeper and Kafka brokers.
- Explored the possibilities of event-driven messaging using Kafka.

### Step 12 - Dockerizing The Application

- Introduced multi-stage builds for optimized Docker images.
- Configured Dockerfile for layered builds to reduce image size.
- Integrated Google's Jib library for efficient image generation.
- Ensured proper port configuration and DNS resolution for Docker containers.

## License

This project is licensed under the GNU General Public License v3.0 (GPL-3.0). You can find the full text of the license [here](https://www.gnu.org/licenses/gpl-3.0.en.html).

---

Thank you for exploring the Microservices Project README! If you have any questions or suggestions, feel free to contact..
