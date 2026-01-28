# Manual REST API Testing with Postman

## Project Overview
Manual functional testing of REST APIs using Postman to validate endpoints, responses, and data integrity across 3 public APIs.

## Status
Project completed - All 22 test cases executed

## APIs Under Test

**JSONPlaceholder** - Social platform simulation  
Base URL: https://jsonplaceholder.typicode.com  
Resources tested: /users, /posts

**ReqRes** - User management CRUD operations  
Base URL: https://reqres.in/api  
Resources tested: /users, /register, /login

**DummyJSON** - E-commerce with authentication  
Base URL: https://dummyjson.com  
Resources tested: /products, /auth/login, /products/search

## Test Results Summary

- **Total Test Cases:** 22
- **Executed:** 22
- **Passed:** 22
- **Pass Rate:** 100%
- **Validation Issues Found:** 1 (low severity)

## Test Scope

- REST API testing (GET, POST, PUT, DELETE, PATCH)
- Status code validation (2xx, 4xx, 5xx)
- Response schema validation
- Authentication testing
- Negative and boundary testing

## Skills Demonstrated

- Manual API testing methodology
- HTTP protocol understanding
- JSON response validation
- API documentation analysis
- Test case design (positive, negative, boundary)
- Postman proficiency (Collection Runner, request configuration)
- Professional test reporting
- Validation issue identification

## Project Structure
```
P4-API-Testing-REST-Postman/
├── README.md
├── .gitignore
├── postman-collections/          # 3 Postman collection exports
│   ├── JSONPlaceholder.postman_collection.json
│   ├── ReqRes.postman_collection.json
│   └── DummyJSON.postman_collection.json
├── test-cases/                   # 22 test case documentation
│   └── API-Test-Cases.md
├── test-results/                 # Execution results & evidence
│   ├── Test-Execution-Summary.md
│   └── screenshots/
│       ├── runner-jsonplaceholder-results.jpg
│       ├── tc03-validation-404.jpg
│       ├── tc04-post-create-201.jpg
│       └── tc20-login-token.jpg
└── documentation/                # Setup guides & API reference
    ├── Postman-Setup-Guide.md
    └── API-Endpoints-Reference.md
```

## How to Run

1. Install Postman Desktop App
2. Import collections from `/postman-collections` folder
3. Follow test cases in `/test-cases/API-Test-Cases.md`
4. Execute requests and verify results

## Test Environment

- **Tool:** Postman v11.x
- **Testing Type:** Manual functional API testing
- **Date:** January 2026
- **QA Tester:** Artur Dmytriyev

## Key Findings

**Validation Issue Identified:**
- Empty 404 response bodies in JSONPlaceholder API lack error context
- Recommendation: Include descriptive error messages in 404 responses

**Positive Outcomes:**
- All endpoints return correct HTTP status codes
- Response structures match API documentation
- Authentication mechanisms work as expected
- Average response time: 187-211ms (excellent performance)

---

**Note:** This project demonstrates systematic manual API testing approach, professional documentation, and ability to identify API design improvements while validating functional correctness.