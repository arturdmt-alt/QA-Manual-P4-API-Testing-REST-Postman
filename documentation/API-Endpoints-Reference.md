# API Endpoints Reference

Quick reference for all endpoints tested in this project.

---

## JSONPlaceholder API

**Base URL:** https://jsonplaceholder.typicode.com

**Endpoints tested:**

**GET /users**  
Returns all users (array of 10 user objects)

**GET /users/{id}**  
Returns single user by ID  
Example: /users/1

**GET /posts**  
Returns all posts (array of 100 post objects)

**POST /posts**  
Creates a new post  
Required fields: title, body, userId

**PUT /posts/{id}**  
Updates an existing post  
Required fields: id, title, body, userId

**DELETE /posts/{id}**  
Deletes a post by ID  
Example: /posts/1

---

## ReqRes API

**Base URL:** https://reqres.in/api

**Endpoints tested:**

**GET /users?page={n}**  
List users with pagination  
Example: /users?page=1 returns page 1 of users

**GET /users/{id}**  
Get single user by ID  
Example: /users/2

**POST /users**  
Create a new user  
Required fields: name, job

**PUT /users/{id}**  
Update existing user  
Required fields: name, job

**DELETE /users/{id}**  
Delete user by ID  
Returns 204 No Content

**POST /register**  
Register a new user  
Required fields: email, password  
Returns token on success

**POST /login**  
User authentication  
Required fields: email, password  
Returns token on success

---

## DummyJSON API

**Base URL:** https://dummyjson.com

**Endpoints tested:**

**GET /products**  
Returns all products (30 products by default)  
Includes: id, title, price, description, category, etc.

**GET /products/{id}**  
Get single product by ID  
Example: /products/1

**POST /products/add**  
Add a new product  
Required fields: title  
Optional: price, description, etc.

**PUT /products/{id}**  
Update existing product  
Example: /products/1

**DELETE /products/{id}**  
Delete product by ID  
Returns deleted product data

**POST /auth/login**  
User login  
Required: username, password  
Test credentials: username='emilys', password='emilyspass'  
Returns: token + user data

**GET /products/search?q={query}**  
Search products by keyword  
Example: /products/search?q=phone  
Returns filtered products array

---

## Notes
- All endpoints support JSON request/response format
- JSONPlaceholder is a fake API - POST/PUT/DELETE won't persist data
- ReqRes provides realistic delayed responses
- DummyJSON requires valid test credentials for auth endpoints

