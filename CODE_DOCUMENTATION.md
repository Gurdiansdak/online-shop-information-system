# 📘 Code Documentation

**Project:** Online Shop Information System  
**Author:** Belek Alisherov  
**Student ID:** 55879  

---

## 1. Overview

This document provides technical documentation of the Online Shop Information System. Its purpose is to describe the internal structure of the system, core components, services, and their interactions. The system is designed using the MVC architectural pattern and RESTful services.

---

## 2. Architectural Overview

The system follows the Model–View–Controller (MVC) architecture:

- **Model** – contains business logic and data entities  
- **View** – user interface layer  
- **Controller** – handles HTTP requests and coordinates services  

The backend is implemented using Node.js with Express and exposed via REST API endpoints.

---

## 3. Core Data Models

### 3.1 User

**Attributes:**
- userId : Integer  
- name : String  
- email : String  
- passwordHash : String  
- role : String (USER / ADMIN)

**Responsibilities:**
- Store user information  
- Support authentication and authorization  

---

### 3.2 Product

**Attributes:**
- productId : Integer  
- name : String  
- description : String  
- price : Decimal  
- category : String  
- stockQuantity : Integer  

**Responsibilities:**
- Store product data  
- Enable product browsing and searching  

---

### 3.3 Cart

**Attributes:**
- cartId : Integer  
- userId : Integer  
- items : List<CartItem>  

**Responsibilities:**
- Manage shopping cart items  
- Calculate total order value  

---

### 3.4 Order

**Attributes:**
- orderId : Integer  
- userId : Integer  
- orderDate : Date  
- totalAmount : Decimal  
- status : String  

**Responsibilities:**
- Store order history  
- Track order lifecycle  

---

### 3.5 Payment

**Attributes:**
- paymentId : Integer  
- orderId : Integer  
- paymentMethod : String  
- paymentStatus : String  

**Responsibilities:**
- Process simulated payments  
- Store payment results  

---

## 4. Services Description

### User Service
- Handles user registration and authentication  

Endpoints:
- POST /api/users/register  
- POST /api/users/login  

---

### Product Service
- Manages product data  

Endpoints:
- GET /api/products  
- POST /api/products  

---

### Cart Service
- Manages shopping cart operations  

Endpoints:
- POST /api/cart/add  
- DELETE /api/cart/remove  

---

### Order Service
- Handles order creation and retrieval  

Endpoints:
- POST /api/orders  
- GET /api/orders/{userId}  

---

### Payment Service
- Simulates online payment process  

Endpoints:
- POST /api/payments  

---

## 5. REST API Example

**Request:**
```json
POST /api/orders
{
  "userId": 1,
  "cartId": 5
}
**Respons:**
{
  "orderId": 21,
  "status": "CREATED",
  "totalAmount": 199.99
}
6. Design Patterns Used
Singleton Pattern

Used for managing database connections to ensure a single shared instance.

Factory Pattern

Used in the payment module to create different payment methods dynamically.

7. Testing Approach

Unit testing is applied conceptually using Jest.

Tested components:

User authentication

Product retrieval

Cart operations

Order creation

8. Summary

This documentation demonstrates a modular system design, clear separation of responsibilities, and adherence to software engineering best practices. The documented structure supports scalability, maintainability, and future extension.
