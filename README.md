# Manual API Testing with Postman

## 📌 Project Overview

This project demonstrates **manual REST API testing using Postman**. The APIs were tested by performing CRUD operations and validating request data, response data, HTTP status codes, headers, and error responses.

The project is designed to demonstrate practical knowledge of **REST API testing and Postman**.

## 🛠️ Tools & Technologies

* **Postman** – API testing
* **REST API** – API architecture
* **JSON** – Request and response data format
* **Git** – Version control
* **GitHub** – Source code and project repository

## 🔄 CRUD Operations Tested

| Operation | HTTP Method | Purpose                     |
| --------- | ----------- | --------------------------- |
| Create    | POST        | Create a new resource       |
| Read      | GET         | Retrieve resource details   |
| Update    | PUT         | Update an existing resource |
| Delete    | DELETE      | Delete a resource           |

## 🧪 Testing Performed

### Functional Testing

* Verified API functionality for CRUD operations
* Validated request payloads
* Validated response payloads
* Verified expected API behavior

### Status Code Validation

Validated appropriate HTTP response codes, including:

* `200 OK`
* `201 Created`
* `400 Bad Request`
* `404 Not Found`

### Request Validation

* Request URL
* HTTP method
* Headers
* Query parameters
* Path parameters
* Request body

### Response Validation

* Response status code
* Response body
* Response headers
* Response structure
* Response data

### Positive Test Scenarios

* Valid request data
* Valid resource ID
* Successful resource creation
* Successful resource retrieval
* Successful resource update
* Successful resource deletion

### Negative Test Scenarios

* Invalid request data
* Invalid resource ID
* Missing required fields
* Invalid parameters
* Non-existing resource requests

## 📂 Project Structure

```text
Manual-API-Testing-Postman/
│
├── postman/
│   └── Manual_API_Testing.postman_collection.json
│
└── README.md
```

## 📦 Postman Collection

The exported Postman collection is available in the `postman` folder.

You can import the collection into Postman and execute the API requests to reproduce the testing scenarios.

## 🎯 Key Learning Outcomes

* Understanding REST API architecture
* Working with HTTP methods
* Performing CRUD operations
* Validating API requests and responses
* Understanding HTTP status codes
* Performing positive and negative API testing
* Using Postman for manual API testing
* Managing API testing collections
* Using Git and GitHub for version control

## 👩‍💻 Author

**Archana**

QA Engineer | Automation & API Testing

GitHub: https://github.com/Archana4GitHub

