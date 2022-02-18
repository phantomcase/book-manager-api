# 📖 Minimalist Book Manager API

## Introduction
This is the starter repository for the Further APIs session. It provides a start to creating a Minimalist Book Manager API
using a Test-Driven Development approach.

### Pre-Requisites
- Java SE Development Kit 11
- Maven

### Technologies & Dependencies
- Spring Boot
- Spring Web
- H2 Database
- Lombok
- Spring Data JPA

### How to Get Started
- Fork this repo to your Github and then clone the forked version of this repo

### Main Entry Point
- The Main Entry Point for the application is: [BookmanagerApplication.java](src/main/java/com/techreturners/bookmanager/BookmanagerApplication.java)

### Running the Unit Tests
- You can run the unit tests in IntelliJ, or you can go to your terminal and inside the root of this directory, run:

`mvn test`

### Tasks

Here are some tasks for you to work on:

📘 Task 1: Implement the following User Story with tests.

`User Story: As a user, I want to use the Book Manager API to delete a book using its ID`


📘 Extension Task: Oh no! 😭 We've only covered the happy paths in the solution, can you figure out a way
to add in exception handling to the project? 

- Clue 1: What if someone wants to add a book with an ID for a book that already exists? How do we handle this gracefully?


- Clue 2: What if someone wants to find a book by an ID that doesn't yet exist? 
  How can we improve the API by handling errors gracefully and show a helpful message to the client?
  

////////////////////////////////////////////////
# USAGE
This is Minimalist Book Manager API
Follow is the endpoint to use for specific function

## Get All Books
### Request
`GET /api/v1/book/`
### Response
  Status: 200 OK
  
  [
  {
  "id": 1,
  "title": "Book title 1",
  "description": "Book Description 1",
  "author": "Author 1",
  "genre": "Romance"
  },
  {
  "id": 2,
  "title": "Book title 2",
  "description": "Book Description 2",
  "author": "Author 2",
  "genre": "Romance"
  },
  {
  "id": 3,
  "title": "Book title 3",
  "description": "Book Description 3",
  "author": "Author 3",
  "genre": "Romance"
  }
  ]

## Get a Book by ID
### Request
`GET /api/v1/book/:id`
### Response
  Status: 200 OK
  
  {
  "id": 1,
  "title": "Book title 1",
  "description": "Book Description 1",
  "author": "Author 1",
  "genre": "Romance"
  }

## Add a Book
### Request
`POST /api/v1/book/`

  book:{
  "title": "Book title 1",
  "description": "Book Description 1",
  "author": "Author 1",
  "genre": "Romance"
  }

### Response
  Status: 201 OK

  {
  "id": 1,
  "title": "Book title 1",
  "description": "Book Description 1",
  "author": "Author 1",
  "genre": "Romance"
  }

## Update a Book
### Request
`PUT /api/v1/book/:id`
### Response
  Status: 200 OK

  {
  "id": 1,
  "title": "Book title 001",
  "description": "Book Description 001",
  "author": "Author 001",
  "genre": "Romance"
  }
  

## Delete a Book
### Request
`DELETE /api/v1/book/:id`
### Response
  Status: 200 OK
