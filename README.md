# Todo API Application

A RESTful API for managing todo tasks with user authentication and persistent storage.

## Features

- User authentication (JWT-based)
- CRUD operations for tasks
- Secure password storage
- Input validation
- Error handling
- Persistent data storage

## Project Structure

/
├── src/
│ ├── controllers/
│ │ ├── authController.js
│ │ └── taskController.js
│ ├── models/
│ │ ├── User.js
│ │ └── Task.js
│ ├── middleware/
│ │ ├── auth.js
│ │ └── validation.js
│ ├── routes/
│ │ ├── authRoutes.js
│ │ └── taskRoutes.js
│ └── app.js
├── .env
├── package.json
└── README.md

## Tech Stack

- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)
- **Password Hashing**: bcrypt
- **Validation**: express-validator

## API Endpoints

### Authentication

- POST /api/auth/signup - Register a new user
- POST /api/auth/login - Login user

### Tasks

- GET /api/tasks - Get all tasks for authenticated user
- POST /api/tasks - Create a new task
- GET /api/tasks/:id - Get specific task
- PUT /api/tasks/:id - Update task
- DELETE /api/tasks/:id - Delete task

## Project Setup

1. Install dependencies:

```bash
npm install
```
