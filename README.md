# Student Records API

A beginner REST API built with Spring Boot and MySQL to store student records.

## Features
- Add a student: POST /students
- List all students: GET /students
- Find one student by id: GET /students/{id}
- Delete a student: DELETE /students/{id}

## Tech used
Java, Spring Boot, Spring Data JPA, MySQL (XAMPP), Maven

## How to run
1. Start MySQL in XAMPP and create a database named `student_db`.
2. Check `src/main/resources/application.properties` (user `root`, empty password).
3. In the project folder, run `.\mvnw.cmd spring-boot:run` (Windows).
4. Open http://localhost:8080/students in your browser.

## Example: add a student (PowerShell)
```
Invoke-RestMethod -Uri http://localhost:8080/students -Method Post -ContentType "application/json" -Body '{"name":"Asha","email":"asha@example.com","course":"MBA"}'
```

## What I learned
- An entity class becomes a database table
- A repository saves and reads data
- A controller turns web requests into actions
