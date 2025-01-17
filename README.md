# Microservice Application: Department and Employee Management
## Demo Video Link : https://drive.google.com/file/d/10G3CPoWjZJq0vMPg_BtqjXOfF5mRDUVl/view?usp=drive_link
## Overview
This project is a microservice-based application developed using Spring Boot. It consists of the following components:

1. **Department Service**: Manages department-related information.
2. **Employee Service**: Manages employee-related information.
3. **Service Registry**: A Eureka Server is used to register and discover the microservices.

The application leverages the Spring Cloud ecosystem and uses Postman for API testing.

---

## Features
- **Microservices Architecture**: Independent Department and Employee services.
- **Service Discovery**: Centralized service registry with Eureka Server.
- **Inter-service Communication**: REST API communication between microservices.
- **API Testing**: Postman is used for testing and verifying endpoints.

---

## Technologies Used
- **Java**: Core programming language.
- **Spring Boot**: Framework for building microservices.
- **Spring Cloud Netflix Eureka**: For service discovery and registry.
- **H2 Database**: In-memory database for development and testing.
- **Postman**: For API testing.
- **Maven**: Dependency management and build tool.

---

## Prerequisites
1. **Java JDK** (version 11 or above)
2. **Maven**
3. **Postman**

---



---

## Setup and Run

### 1. Clone the Repository
```bash
git clone <repository-url>
cd <project-folder>
```

### 2. Run the Service Registry
```bash
cd service-registry
mvn spring-boot:run
```

### 3. Run the Department Service
```bash
cd ../department-service
mvn spring-boot:run
```

### 4. Run the Employee Service
```bash
cd ../employee-service
mvn spring-boot:run
```

---

## API Endpoints

### Department Service
- **Create Department**: `POST /departments`
- **Get Department by ID**: `GET /departments/{id}`

### Employee Service
- **Create Employee**: `POST /employees`
- **Get Employee by ID**: `GET /employees/{id}`
- **Get Employee by Department**: `GET /employees/department/{departmentId}`

---

## Testing with Postman
1. Import the provided Postman collection into Postman.
2. Use the following base URLs for testing:
   - **Department Service**: `http://localhost:<port>/departments`
   - **Employee Service**: `http://localhost:<port>/employees`
3. Test the endpoints using appropriate HTTP methods and payloads.

---

## Eureka Server
- Access the Eureka Dashboard at `http://localhost:<eureka-port>`.
- Verify that the Department and Employee services are registered.

---

## Future Enhancements
- Add a centralized API Gateway.
- Implement security with Spring Security and JWT.
- Integrate with an external database.

---

## Contributors
- [Your Name] (Project Owner)

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

