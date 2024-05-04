# Spring

## Challenge
 Develop a backend service for managing a library of books using Spring Boot with Spring WebFlux or Spring MVC.

## Requirements

1. **Book Entity:**
- Create a Book entity with the following fields: id (auto-generated), title, author, publicationYear, and availableCopies.

2. **CRUD Operations:**
- Implement CRUD (Create, Read, Update, Delete) operations for managing books.
- Include endpoints for adding a new book, retrieving a book by ID, updating book details, and deleting a book.

3. **Persistence:**
- **Reactive Database**
    - Use Spring Data Reactive MongoDB or any reactive database to persist book entities.
- or **Relational Database**
    - Use Spring Data JPA to persist book entities to a relational database (e.g. H2).
- Configure appropriate database connection properties in the application.properties file.

4. **RESTful API:**
- **Spring WebFlux**
    - Expose the CRUD operations as RESTful endpoints using Spring WebFlux annotations.
    - Utilize reactive programming with Spring WebFlux to achieve non-blocking I/O and scalability.
- or **Spring MVC**
    - Expose the CRUD operations as RESTful endpoints using Spring MVC annotations.
    - Use synchronous request handling with Spring MVC to process HTTP requests and responses.

5. **Error Handling:**
- Implement error handling for invalid requests, missing resources, and other exceptional scenarios. Return meaningful error messages and appropriate HTTP status codes.

6. **Testing:**
- Write unit tests to verify the functionality of the CRUD operations.
- Use tools like JUnit, Mockito, and WebTestClient for writing and executing tests.

**Timeframe**: Between 1 to 2 hours.

**Submission**: Once completed, push your project source code to a public GitHub repository. Document instructions for building and running the application and take screenshots of the test results.
