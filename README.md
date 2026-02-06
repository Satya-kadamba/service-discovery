# Microservices Demo

A simple **Spring Boot Microservices** demo project that showcases how independent services communicate with each other using REST, service discovery, and centralized configuration.

This project is intended for **learning, demos, and interview preparation**.

---

## Architecture Overview

The demo follows a classic microservices architecture:

* Independent services with their own databases
* Service-to-service communication using REST
* Centralized configuration
* Service discovery

```
Client
  |
  v
Service Discovery (Eureka)
  |
  +--> User Service
  |
  +--> Product Service
```

---

## Services Included

### 1. Service Registry (Eureka Server)

* Registers all microservices
* Enables service discovery
* Eliminates hard-coded service URLs

**Port:** `8761`

---

### 2. User Service

* Manages user-related operations
* Independent database
* Exposes REST APIs

**Port:** `8081`

---

### 3. Product Service

* Manages product information
* Independent database
* Exposes REST APIs

**Port:** `8082`

---


## Tech Stack

* Java 17
* Spring Boot
* Spring Cloud
* Spring Data JPA
* Eureka Discovery Server
* Spring Cloud Config
* Spring Cloud Gateway
* REST APIs
* Maven
* MySQL / H2 (for demo)

---

## Prerequisites

* Java 17+
* Maven 3.8+
* Git
* IDE (IntelliJ IDEA / Eclipse)

---

## How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <repository-url>
cd microservices-demo
```

---

### Step 2: Start Eureka Server

```bash
cd eureka-server
mvn spring-boot:run
```

Verify: `http://localhost:8761`

---

### Step 3: Start Microservices

Run each service in a separate terminal:

```bash
cd user-service
mvn spring-boot:run
```

```bash
cd product-service
mvn spring-boot:run
```
---

## Sample API Endpoints

### User Service

```
GET /users
POST /users
```

### Product Service

```
GET /products
POST /products
```

## Key Microservices Concepts Demonstrated

* Service Discovery
* Centralized Configuration
* API Gateway Routing
* Loose Coupling
* Independent Deployment
* Scalability
* Fault Isolation

---

## Common Issues

* Ensure Config Server starts before other services
* Check service registration in Eureka dashboard
* Verify correct application name in `spring.application.name`

---

## Future Enhancements

* Security using Spring Security & JWT
* Circuit Breaker (Resilience4j)
* Distributed Tracing (Zipkin)
* Docker & Docker Compose
* Kubernetes deployment

---

## License

This project is for educational purposes only.# Microservices Demo

A simple **Spring Boot Microservices** demo project that showcases how independent services communicate with each other using REST, service discovery, and centralized configuration.

This project is intended for **learning, demos, and interview preparation**.

---

## Architecture Overview

The demo follows a classic microservices architecture:

* Independent services with their own databases
* Service-to-service communication using REST
* Centralized configuration
* Service discovery

```
Client
  |
  v
Service Discovery (Eureka)
  |
  +--> User Service
  |
  +--> Product Service
  |
  +--> Order Service
```

---

## Services Included

### 1. Service Registry (Eureka Server)

* Registers all microservices
* Enables service discovery
* Eliminates hard-coded service URLs

**Port:** `8761`

---

### 2. User Service

* Manages user-related operations
* Independent database
* Exposes REST APIs

**Port:** `8081`

---

### 3. Product Service

* Manages product information
* Independent database
* Exposes REST APIs

**Port:** `8082`

---


## Tech Stack

* Java 17
* Spring Boot
* Spring Cloud
* Spring Data JPA
* Eureka Discovery Server
* Spring Cloud Config
* Spring Cloud Gateway
* REST APIs
* Maven
* MySQL / H2 (for demo)

---

## Prerequisites

* Java 17+
* Maven 3.8+
* Git
* IDE (IntelliJ IDEA / Eclipse)

---

## How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <repository-url>
cd microservices-demo
```

---

### Step 2: Start Eureka Server

```bash
cd eureka-server
mvn spring-boot:run
```

Verify: `http://localhost:8761`

---

### Step 3: Start Microservices

Run each service in a separate terminal:

```bash
cd user-service
mvn spring-boot:run
```

```bash
cd product-service
mvn spring-boot:run
```
---

## Sample API Endpoints

### User Service

```
GET /users
POST /users
```

### Product Service

```
GET /products
POST /products
```

## Key Microservices Concepts Demonstrated

* Service Discovery
* Centralized Configuration
* API Gateway Routing
* Loose Coupling
* Independent Deployment
* Scalability
* Fault Isolation

---

## Common Issues

* Ensure Config Server starts before other services
* Check service registration in Eureka dashboard
* Verify correct application name in `spring.application.name`

---

## Future Enhancements

* Security using Spring Security & JWT
* Circuit Breaker (Resilience4j)
* Distributed Tracing (Zipkin)
* Docker & Docker Compose
* Kubernetes deployment

---

## License

This project is for educational purposes only.
