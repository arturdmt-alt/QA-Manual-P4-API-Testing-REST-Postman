# API Test Cases - REST API Testing

## Test Case Summary
- **Total Test Cases:** 22
- **Status:** Not Executed
- **APIs Covered:** JSONPlaceholder, ReqRes, DummyJSON

---

## JSONPlaceholder API

### TC01: GET All Users - Verify 200 Response
**Endpoint:** GET /users  
**Expected:** Status 200, Array of user objects  
**Status:** Not Executed

### TC02: GET Single User by ID - Valid ID
**Endpoint:** GET /users/1  
**Expected:** Status 200, User object with id=1  
**Status:** Not Executed

### TC03: GET User by Invalid ID - 404 Test
**Endpoint:** GET /users/999999  
**Expected:** Status 404 or empty response  
**Status:** Not Executed

### TC04: POST Create New Post
**Endpoint:** POST /posts  
**Body:** { title, body, userId }  
**Expected:** Status 201, Created post object  
**Status:** Not Executed

### TC05: PUT Update Existing Post
**Endpoint:** PUT /posts/1  
**Body:** { id, title, body, userId }  
**Expected:** Status 200, Updated post object  
**Status:** Not Executed

### TC06: DELETE Post
**Endpoint:** DELETE /posts/1  
**Expected:** Status 200 or 204  
**Status:** Not Executed

---

## ReqRes API

### TC07: GET List Users with Pagination
**Endpoint:** GET /api/users?page=1  
**Expected:** Status 200, Paginated user data  
**Status:** Not Executed

### TC08: GET Single User - Valid ID
**Endpoint:** GET /api/users/2  
**Expected:** Status 200, User object  
**Status:** Not Executed

### TC09: GET User Not Found - 404
**Endpoint:** GET /api/users/23  
**Expected:** Status 404  
**Status:** Not Executed

### TC10: POST Create User
**Endpoint:** POST /api/users  
**Body:** { name, job }  
**Expected:** Status 201, Created user with id  
**Status:** Not Executed

### TC11: PUT Update User
**Endpoint:** PUT /api/users/2  
**Body:** { name, job }  
**Expected:** Status 200, Updated user object  
**Status:** Not Executed

### TC12: DELETE User
**Endpoint:** DELETE /api/users/2  
**Expected:** Status 204 No Content  
**Status:** Not Executed

### TC13: POST Register Successful
**Endpoint:** POST /api/register  
**Body:** { email, password }  
**Expected:** Status 200, Token returned  
**Status:** Not Executed

### TC14: POST Register Unsuccessful - Missing Password
**Endpoint:** POST /api/register  
**Body:** { email } (no password)  
**Expected:** Status 400, Error message  
**Status:** Not Executed

---

## DummyJSON API

### TC15: GET All Products
**Endpoint:** GET /products  
**Expected:** Status 200, Array of products  
**Status:** Not Executed

### TC16: GET Single Product
**Endpoint:** GET /products/1  
**Expected:** Status 200, Product object  
**Status:** Not Executed

### TC17: POST Add New Product
**Endpoint:** POST /products/add  
**Body:** { title, price }  
**Expected:** Status 200, Created product  
**Status:** Not Executed

### TC18: PUT Update Product
**Endpoint:** PUT /products/1  
**Body:** { title, price }  
**Expected:** Status 200, Updated product  
**Status:** Not Executed

### TC19: DELETE Product
**Endpoint:** DELETE /products/1  
**Expected:** Status 200, Deleted product confirmation  
**Status:** Not Executed

### TC20: POST Login Successful
**Endpoint:** POST /auth/login  
**Body:** { username: 'emilys', password: 'emilyspass' }  
**Expected:** Status 200, Token + user data  
**Status:** Not Executed

### TC21: POST Login Failed - Invalid Credentials
**Endpoint:** POST /auth/login  
**Body:** { username: 'invalid', password: 'wrong' }  
**Expected:** Status 400/401, Error message  
**Status:** Not Executed

### TC22: GET Search Products
**Endpoint:** GET /products/search?q=phone  
**Expected:** Status 200, Filtered products array  
**Status:** Not Executed

---

## Test Case Summary by Type
- **Positive Tests:** 14
- **Negative Tests:** 6
- **Boundary Tests:** 2
- **Authentication Tests:** 4
