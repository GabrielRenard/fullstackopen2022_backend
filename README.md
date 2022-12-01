# FullStackOpen 2022 Backend

## 1. [Node.js & Express](#Node.js-&-Express)

- ### [Introduction](##Introduction)
- ### [Topics Learnt](##Topics-Learnt)
- ### [Project](##Project)
  - #### [Criteria](###Criteria)

## Node.js & Express

### Introduction

---

#### This part of the course focuses on the backend using the **Node JS** Javascript runtime and the **Express** library. The goal is to learn how to implement a backend to the phonebook project from part 2 of the course (Communicating with Server).

### Topics Learnt

---

- #### Creating a Web Server Using Node.js
- #### Implementing Server Side Code Using Express
- #### Transitive Dependencies & Semantic Versioning
- #### HTTP Request Methods & Working With Reponse Data
- #### Nodemon & Hot Reloads
- #### Representational State Transfer (REST)
- #### HTTP Status Codes & Error Handling
- #### Postman & VS Code REST Client for Testing
- #### HTTP Standards: Safety & Idempotence
- #### Middlewares

### Project

---

#### Criteria

---

#### 1. Implement a Node application that returns a hardcoded list of phonebook entries.

- ##### The application must be started with the command `npm start`.

- ##### The application must also offer an `npm run dev` command that will run the application and restart the server whenever changes are made and saved to a file in the source code.

#### 2. Implement a page at _http://localhost:3001/info_ which shows the time that the request was received and how many entries are in the phonebook at the time of processing the request.

#### 3. Implement the functionality for displaying the information for a single phonebook entry.

- ##### If an entry for the given id is not found, the server has to respond with the appropriate status code.

#### 4. Implement functionality that makes it possible to delete a single phonebook entry by making an HTTP DELETE request to the unique URL of that phonebook entry.

- ##### Test that your functionality works with either Postman or the Visual Studio Code REST client.

#### 5. Expand the backend so that new phonebook entries can be added by making HTTP POST requests to the address _http://localhost:3001/api/persons_.

- ##### Generate a new id for the phonebook entry with the Math.random function. Use a big enough range for your random values so that the likelihood of creating duplicate ids is small.

#### 6. Implement error handling for creating new entries. The request is not allowed to succeed, if:

1. ##### The name or number is missing.
2. ##### The name already exists in the phonebook

- ##### Respond to requests like these with the appropriate status code, and also send back information that explains the reason for the error, e.g.:
