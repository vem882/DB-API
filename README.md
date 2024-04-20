# Databases and Interfaces Course Project

This repository contains a web application developed as part of the "Databases and Interfaces" course at Oulu University of Applied Sciences. The application is built using Node.js with Express.js framework and MySQL database, providing web interfaces to manage books and student records.

## Technologies Used
- Node.js
- Express.js
- MySQL
- dotenv for environment variables management
- Additional middleware such as cookie-parser, debug, and morgan for logging and debugging

## Project Structure

- `app.js` - Initializes the app and sets up middleware and routes.
- `database.js` - Database
- `index.js` - Index
- `/models` - Contains models for database operations.
  - `book_model.js` - Handles CRUD operations for books.
  - `student_model.js` - Handles CRUD operations for students.
- `/bin` - Express.js dir
  - `www` - Express.js web-server settings.
- `/routes` - Defines the router for handling requests.
  - `index.js` - Root router.
  - `book.js` - Router for book-related operations.
  - `student.js` - Router for student-related operations.
  


## Setup

To get this project up and running, follow these steps:

1. Clone the repository:
   ```
   git clone [repository-url]
   ```
2. Install dependencies:
   ```
   npm install
   ```
3. Configure your MySQL database settings in an `.env` file based on the `.env.example` provided in the repository.
4. Start the application:
   ```
   npm start
   ```

## API Usage

The application exposes several endpoints for interacting with the database:

### Books
- `GET /book` - Retrieves all books.
- `GET /book/:id` - Retrieves a book by its ID.
- `POST /book` - Adds a new book. Requires `name`, `author`, and `isbn`.
- `DELETE /book/:id` - Deletes a book by its ID.
- `PUT /book/:id` - Updates an existing book. Requires `name`, `author`, and `isbn`.

### Students
- `GET /student` - Retrieves all students.
- `GET /student/:id` - Retrieves a student by ID.
- `POST /student` - Adds a new student. Requires data specific to your project needs.
- `DELETE /student/:id` - Deletes a student by ID.
- `PUT /student/:id` - Updates an existing student. Requires data specific to your project needs.

## Contributing

Contributions to this project are welcome. Please fork the repository and submit a pull request with your changes or suggestions.

---
