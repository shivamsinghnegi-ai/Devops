# demo - Spring Boot CRUD example

This repository contains a minimal Spring Boot CRUD application and a `Jenkinsfile` for CI.

Run locally

Install JDK 17 and Maven.

Build and run tests:

```bash
mvn -B clean package
```

Run the app:

```bash
mvn spring-boot:run


GVKQEDwl,.;,vkt0[5e]
jtyqwku.niedj.mot
# or
java -jar target/demo-0.0.1-SNAPSHOT.jar
```

API endpoints (default port 8080):

- `GET /api/books` - list all books
- `GET /api/books/{id}` - get book
- `POST /api/books` - create (JSON body: title, author)
- `PUT /api/books/{id}` - update
- `DELETE /api/books/{id}` - delete

Jenkins pipeline

The included `Jenkinsfile` checks out the repo, builds with Maven, runs tests and archives `target/*.jar`.
