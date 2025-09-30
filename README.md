# bookstoreRESTfulAPI
This project was created as part of my university coursework. It implements a RESTful Bookstore API in Java JAX-RS, with resources for authors, books, customers, carts, and orders, fully tested and documented in an accompanying report.

---

## Features  

- **Author Resource**  
  - Create, update, delete, and fetch authors.  
  - Retrieve books linked to a specific author.  
  - Validates required fields and handles missing/invalid IDs.  

- **Book Resource**  
  - Full CRUD operations for books.  
  - Validates constraints such as non-negative prices and realistic publication years.  
  - Ensures author references exist.  

- **Customer Resource**  
  - Manage customer accounts with basic validation (name, email, password).  
  - Supports updates and deletions, with error handling for invalid data.  

- **Cart Resource**  
  - Add, update, or remove items in a customer’s shopping cart.  
  - Validates stock availability and customer existence.  
  - Retrieves full cart contents for each customer.  

- **Order Resource**  
  - Place orders from a customer’s cart.  
  - Ensures carts are valid and non-empty before creating orders.  
  - Fetch all orders by customer or retrieve a specific order.  

---

## Testing  

- The API was thoroughly tested using **Postman**.  
- Tests cover **happy paths, invalid inputs, and error conditions**.  
- Results are documented in the report with tables for each resource, including:  
  - HTTP method and endpoint  
  - Request body (if applicable)  
  - Expected status and response  
  - Actual result (Pass/Fail)  

---

## Technologies Used  

- **Java EE 8 (JAX-RS)** – REST API framework  
- **JSON** – request/response format  
- **In-memory storage** – `ArrayList`, `HashMap`  
- **Postman** – API testing  

---

## How to Run  

1. Clone this repository:  
   ```bash
   git clone https://github.com/Mgilgil/BookstoreAPI.git
  2. Open the project in your preferred Java EE 8–compatible IDE or application server (e.g., NetBeans).
  3. Deploy and run the server.
  4. Use Postman (or another REST client) to interact with endpoints such as: POST /customers/{id}/cart/items
