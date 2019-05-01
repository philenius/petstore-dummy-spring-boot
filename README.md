# Petstore Dummy Spring Boot

Dummy implementation of Petstore OpenAPI 3.0 spec using Spring Boot. This server was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project. The underlying library integrating swagger to SpringBoot is [springfox](https://github.com/springfox/springfox).

## Build

```bash
docker build -t petstore-dummy-spring-boot .
```

## Run

```bash
docker run -p 8080:8080 petstore-dummy-spring-boot
```

