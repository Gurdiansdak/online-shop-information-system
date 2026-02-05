# 🧪 Testing Documentation

**Project:** Online Shop Information System  
**Author:** Belek Alisherov  
**Student ID:** 55879  

---

## 1. Testing Strategy

Testing is performed to verify the correctness, reliability, and consistency of the system.  
The following testing levels are applied:

- Unit Testing  
- Integration Testing  

Testing is conceptually implemented using **Jest** for Node.js applications.

---

## 2. Unit Tests

The following system components are covered by unit tests:

- User authentication logic  
- Product retrieval service  
- Shopping cart operations  
- Order creation process  

### Unit Test Cases

| Test ID | Component | Description | Expected Result |
|------|----------|-------------|----------------|
| UT-01 | User Service | Validate user login | Login successful |
| UT-02 | Product Service | Retrieve products | Product list returned |
| UT-03 | Cart Service | Add item to cart | Item added successfully |
| UT-04 | Order Service | Create order | Order created |

---

## 3. Integration Tests

Integration testing verifies interactions between system services.

| Test ID | Scenario | Description | Result |
|------|----------|-------------|--------|
| IT-01 | Order & Payment | Process order payment | Successful |
| IT-02 | User & Cart | Manage cart after login | Successful |

---

## 4. Testing Summary

Testing confirms that the system’s core functionalities work correctly and that services interact reliably.  
The applied testing approach reduces the risk of defects and improves system quality.
