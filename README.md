# 🛒 Online Shop Information System

**Author:** Belek Alisherov  
**Student ID:** 55879  
**Course:** Software Development Methodologies  
**Project Type:** Design and Implementation of an Information System  
**Selected Methodology:** Scrum  

---

## 📌 Project Overview

The *Online Shop Information System* is a web-based information system designed to simulate the functionality of a modern e-commerce platform. The system allows users to browse products, manage a shopping cart, place orders, and perform simulated online payments. An administrative interface enables product management and system supervision.

The main focus of this project is the correct application of **software development methodologies**, **system design**, **UML modeling**, **architectural patterns**, and **technical documentation**, rather than full-scale production deployment.

---

## 🎯 Project Objectives

- Design an information system using a selected software development methodology  
- Define functional and non-functional requirements  
- Apply Scrum methodology in an iterative manner  
- Model the system using UML diagrams  
- Apply architectural and design patterns  
- Design RESTful web services  
- Prepare technical and code documentation  

---

## 🔄 Selected Software Development Methodology – Scrum

Scrum was selected due to its iterative and incremental development approach, flexibility, and suitability for web-based systems.

### Scrum Roles
- **Product Owner** – responsible for defining system requirements and priorities  
- **Development Team** – designs and implements system components  
- **Scrum Master** – ensures proper Scrum process execution  

### Scrum Artifacts
- Product Backlog  
- Sprint Backlog  
- Increment  

### Scrum Events
- Sprint Planning  
- Sprint Review  
- Sprint Retrospective  

---

## 🧩 System Architecture

The system follows the **MVC (Model–View–Controller)** architectural pattern and is divided into **RESTful services**.

### Architecture Layers
- **Model:** business logic and data entities  
- **View:** user interface implemented using HTML, CSS, and JavaScript  
- **Controller:** handles user requests and coordinates communication with services  

### System Services
- User Service  
- Product Service  
- Cart Service  
- Order Service  
- Payment Service  

All services communicate using **HTTP** protocol and **JSON** data format.

---

## 🛠️ Technology Stack

- **Backend:** Node.js (Express)  
- **Frontend:** HTML, CSS, JavaScript  
- **Database:** MySQL  
- **API Style:** REST  
- **Testing:** Jest (conceptual unit testing)  

---

## 📂 Project Structure (Logical)

online-shop-information-system/
│── README.md
│── backend/
│ ├── controllers/
│ ├── services/
│ ├── models/
│ └── tests/
│── frontend/
│ ├── pages/
│ ├── styles/
│ └── scripts/
│── docs/
│ ├── architecture.md
│ ├── api-documentation.md
│ └── uml-diagrams/


---

## 🔐 Functional Overview

### User Features
- User registration and authentication  
- Product browsing and searching  
- Shopping cart management  
- Order placement and order history  

### Admin Features
- Product creation, update, and deletion  
- Order monitoring and management  

---

## 📡 REST API Overview (Examples)

| Method | Endpoint | Description |
|------|---------|-------------|
| POST | /api/users/register | Register a new user |
| POST | /api/users/login | Authenticate user |
| GET | /api/products | Retrieve product list |
| POST | /api/cart | Add product to shopping cart |
| POST | /api/orders | Place a new order |
| POST | /api/payments | Simulate online payment |

---

## 🧪 Testing Strategy

Testing includes unit and integration tests to verify system correctness and reliability.

### Example Unit Tests
- User authentication validation  
- Product retrieval functionality  
- Shopping cart operations  
- Order creation process  

---

## 🧠 Design Patterns Used

- **Singleton Pattern:** used for database connection management to ensure a single shared instance  
- **Factory Pattern:** used to dynamically create different payment methods  

These patterns improve scalability, maintainability, and extensibility of the system.

---

## 🚀 How to Run (Simulation)

1. Install Node.js  
2. Configure the database connection  
3. Start the backend server using `npm start`  
4. Open the frontend in a web browser  

*Note: Full system deployment is not required for this academic project.*

---

## 📈 Future Improvements

- Integration with real payment gateways  
- Mobile application support  
- Advanced security mechanisms  
- Migration to a microservices architecture  

---

## 📚 References

- Software Engineering course materials  
- Scrum Guide  
- REST API Design Guidelines  
