# EmpX - Employee Portal

## Overview

EmpX is a web-based application to manage employee records. It allows users to add, view, edit, and delete employee details. The backend is built using Node.js, Express, and MongoDB, with EJS for dynamic templating.

---

## Quick Start Guide

### Prerequisites
Ensure you have the following installed:
1. Node.js (with npm)
2. MongoDB (running locally or remotely)

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Navigate to the project directory:**
   ```bash
   cd path/to/EmpX
   ```

3. **Install dependencies:**
   ```bash
   npm i
   ```

4. **Start the application:**
   ```bash
   node index.js
   ```

5. **Open the application in your browser:**
   Go to [http://localhost:3000](http://localhost:3000).

---

## Features

### Employee Management
1. **Add Employee:** Fill in the form to add a new employee with fields such as Employee ID, Name, Position, and Salary.
2. **View Employee:** See a list of all employees.
3. **Edit Employee:** Modify the details of an existing employee.
4. **Delete Employee:** Remove an employee from the database.

---

## MongoDB Configuration

The application uses MongoDB for storing employee details. Ensure MongoDB is running locally or provide a connection string in the code:

```javascript
mongoose.connect('mongodb://localhost:27017/emp_x', {
  useNewUrlParser: true,
  useUnifiedTopology: true,
});
```

If using a remote MongoDB instance, replace `localhost:27017/emp_x` with your MongoDB connection string.

---

## Dependencies
The application uses the following npm packages:
1. **express:** Web framework
2. **mongoose:** MongoDB object modeling tool
3. **ejs:** Template engine

---

## API Endpoints

**Base URL:** [http://localhost:3000](http://localhost:3000)

1. **GET /**: Fetch and display all employees.
2. **GET /add:** Show the form to add a new employee.
3. **POST /add:** Create a new employee.
4. **GET /edit/:id:** Fetch employee details for editing.
5. **POST /edit:** Update employee details.
6. **GET /delete/:id:** Delete an employee by ID.

---

## Author

**Rajalakshmi R**
