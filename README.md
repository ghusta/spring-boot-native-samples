# Spring Boot Native Samples

![build](https://github.com/alexcheng1982/spring-boot-native-samples/actions/workflows/build.yml/badge.svg)

Samples of using Spring Boot to build native executables

* Java 17 required (GraalVM Java 17 required for `native` profile)
* Tested with GraalVM 22.2.0 Java 17 CE

## Samples


### gRPC

Simple gRPC service

| Mode | Binary size | Startup time | Memory |
|--------|-------|-------|--|
| JVM | 21.5 (JAR) | 0.835s | 96MB |
| Native | 47.8MB | 0.085s | 17.4MB |

### Spring Data JPA with WebMvc

A microservice with REST API and RDBMS backend

| Mode | Binary size | Startup time | Memory |
|--------|-------|-------|--|
| JVM | 43.5 (JAR) | 2.83s | 183MB |
| Native | 123MB | 0.237s | 64.6MB |

Features:

* Spring Data JPA
* Spring Web MVC
* Flyway
* PostgreSQL
* Testcontainers
* OpenAPI doc & Swagger UI

### Reactive JDBC & WebFlux

A reactive microservice with REST API and RDBMS backend

| Mode | Binary size | Startup time | Memory |
|--------|-------|-------|--|
| JVM | 32.1 (JAR) | 1.929s | 142.7MB |
| Native | 79.4MB | 0.217s | 56.9MB |

Features:

* Spring Data R2dbc
* Spring WebFlux
* Flyway
* PostgreSQL
* Testcontainers
