# student-management-system-remix
A continuation/remake of the [student-management-system](https://github.com/yoanpetrov02/student-management-system) project. The idea is to improve the structure and architecture and add new technologies such as Docker and Kafka, as well as focus on other details like database indexing and migrations.

# Prerequisites

#### You need to have the following tools installed:
- Docker (v24.0.6 was used for development) - [Install](https://docs.docker.com/engine/install/)
- Java 17 - [Install](https://docs.oracle.com/en/java/javase/17/install/overview-jdk-installation.html)

#### Other details
- Make sure you don't have a PostgreSQL or pgAdmin4 server running already/at the same ports as the ones set in `compose.yaml`

# How to run
- Checkout the project.
- Navigate to its root directory (student-management-system-remix).
- Launch the database services:
```
docker compose up
```
- Follow the template from `application-yml-template.txt` to create an `application.yml` file under `src/main/resources`.
- After creating the `application.yml` file, navigate to the server module (Student-Management-System):
```
cd Student-Management-System
```
and launch the server:
  - For windows
  ```
  mvnw.cmd spring-boot:run
  ```
  - For linux
  ```
  ./mvnw spring-boot:run
  ```