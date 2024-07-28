# User Authentication Application

## Objective
The User Authentication Application provides a secure way for users to register and log in. It uses Spring Boot for the backend and Angular for the frontend, with JSON Web Tokens (JWT) to ensure secure access to the system. The goal is to protect resources and manage user authentication efficiently

## Requirements
### Backend Setup (Java with Spring Boot)
1. **Create a Spring Boot Application**
   - Dependencies:
     - Spring Web
     - Spring Security
     - Spring Data JPA
     - jjwt (Java JWT library)

2. **Implement User Authentication**
  # Components  
   - **User Model**: Create a User entity with fields:
     - id
     - username
     - password (store as hashed)
   - **User Repository**: Implement a `UserRepository` interface extending `JpaRepository`.
   - **User Service**: Create a service for user registration and authentication.
   - **JWT Utility**: Create a utility class to generate and validate JWTs.
   - **Security Configuration**: Configure Spring Security to handle authentication and protect routes.
   - **Authentication Controller**:
     - Create an endpoint for user registration.
     - Create an endpoint for user login that returns a JWT upon successful authentication.

### Frontend Setup (Angular)
1. **Create an Angular Application**
   - Dependencies:
     - Angular Router
     - HttpClientModule
     - Angular Material (optional for UI components)

2. **Implement User Interface**
   - **Login Component**: Create a form with username and password fields.
   - **Registration Component**: Create a form for user registration with username and password fields.
   - **Service to Handle HTTP Requests**: Create an `AuthService` to handle login, registration, and JWT storage.

### MySQL Database Configuration

Configure your MySQL database connection in `application.properties`:

properties
spring.datasource.url=jdbc:mysql://localhost:3306/mydatabase?createDatabaseIfNotExist=true.
spring.datasource.username=root.
spring.datasource.password=Narendra@2000.
spring.jpa.hibernate.ddl-auto=update.
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect...

### Prerequisites
- Java Development Kit (JDK) 11 or higher
- Maven
- A relational database (e.g., MYSQL)
- 
## Evaluation Criteria
- Correct implementation of backend authentication logic.
- Proper integration of frontend components.
- Code quality and adherence to best practices.
- Functionality of the application (registration, login, JWT storage).

## Resources
- [Spring Security JWT Documentation](https://spring.io/guides/tutorials/spring-boot-oauth2)
- [Angular HTTP Client Documentation](https://blog.angular-university.io/angular-http/)

## How to Run the Application

### Backend
### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/kuppalanarendra/User_Logiin-Authentication.git

## Contributing
Contributions to the project are welcome! If you have any ideas for improvements or new features, feel free to open an issue or submit a pull request.

## License
  This project is licensed under the MIT License.
  
## Author
Your Name:K.Narendra

## Acknowledgments
  * Special thanks to the Spring Boot community for their excellent documentation and 
  support.
  * Special thanks to Jeev Lifeworks for giving this project for me.

