# Node-Rest-Api-Typescript
This project is a Node.js and TypeScript-based REST API built using Express, MongoDB, and JWT authentication. It provides secure CRUD operations for users, products, and students with validation, rate limiting, and environment configuration.
# Node.js TypeScript REST API

A scalable and production-ready REST API built with Node.js, TypeScript, and Express. This project follows a modular architecture with proper separation of concerns, including controllers, routes, middleware, validation, and database layers.

---

## Overview

This API provides a robust backend foundation with authentication, validation, and security best practices. It is designed for maintainability, scalability, and real-world application development.

---

## Tech Stack

* Node.js
* TypeScript
* Express.js
* MongoDB
* Mongoose
* JWT Authentication
* Joi Validation

---

## Features

* User authentication (Register & Login)
* JWT-based authorization
* Request validation using Joi
* Secure password hashing (Argon2)
* Rate limiting for API protection
* Centralized error handling
* Modular folder structure
* Environment-based configuration
* Logging and security middleware

---

## Project Structure

```
src/
│
├── config/         # Database and environment configuration
├── controllers/    # Business logic
├── interfaces/     # TypeScript interfaces
├── middleware/     # Custom middleware (auth, error, rate limiter)
├── models/         # Mongoose schemas
├── routes/         # API route definitions
├── validation/     # Joi validation schemas
└── server.ts       # Entry point
```

---

## Installation

Clone the repository:

```
git clone https://github.com/nasrin-a-mahin/Node-Rest-Api-Typescript.git
cd Node-Rest-Api-Typescript
```

Install dependencies:

```
npm install
```

---

## Environment Variables

Create a `.env` file in the root directory:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
NODE_ENV=development
```

---

## Running the Application

### Development

```
npm run dev
```

### Build

```
npm run build
```

### Production

```
npm start
```

---

## API Endpoints

### Authentication

**Register**

```
POST /api/auth/register
```

**Login**

```
POST /api/auth/login
```

---

## Sample Request

```
POST /api/auth/register
Content-Type: application/json

{
  "username": "testuser",
  "email": "test@gmail.com",
  "password": "Test@123"
}
```

---

## Security

* Helmet for HTTP headers
* Rate limiting to prevent abuse
* Password hashing using Argon2
* JWT for secure authentication

---

## Code Quality

* ESLint for linting
* Prettier for formatting
* Strict TypeScript configuration

---

## Future Improvements

* Role-based access control (RBAC)
* Refresh token implementation
* API documentation (Swagger)
* Unit and integration testing

---

## License

This project is licensed under the MIT License.
