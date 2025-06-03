# Basic JWT Authentication with Spring Boot 🚀

This is a simple **Spring Boot** application demonstrating **JWT (JSON Web Token) Authentication** to secure REST APIs.

## 📚 Overview
This project:
- Registers and authenticates users with JWT tokens.
- Secures REST API endpoints.
- Demonstrates basic JWT generation, validation, and Spring Security integration.

---

## 🛠️ Technologies Used
- **Spring Boot 3.x**
- **Spring Security**
- **Spring Data JPA**
- **H2 Database**
- **Lombok**
- **JJWT (Java JWT)**

---

## ⚙️ Setup Instructions

### 🔨 Clone the repository
```bash
git clone https://github.com/eneaves/Basic-jwt-authentication.git
cd Basic-jwt-authentication
🏗️ Build and Run
bash
Copiar
Editar
./mvnw clean install
./mvnw spring-boot:run
The application will start on:
📍 http://localhost:8080

🧪 API Endpoints
🔑 Authentication
POST /api/auth/signup – Register a new user.

json
Copiar
Editar
{
  "username": "testuser",
  "password": "testpass"
}
POST /api/auth/signin – Login and obtain a JWT.

json
Copiar
Editar
{
  "username": "testuser",
  "password": "testpass"
}
Response:

php-template
Copiar
Editar
<JWT token>
🔒 Secured Endpoints
GET /api/test/all – Public content.

GET /api/test/user – Requires JWT.
Include the token in the header:

makefile
Copiar
Editar
Authorization: Bearer <your_token>



