# Database Connection

## Module Name
**Database Connection**

## Description

The Database Connection module establishes communication between the backend server and the MySQL database. It enables the application to store, retrieve, update, and delete information related to patients, doctors, appointments, and administrators.

---

# Objective

The objectives of the Database Connection module are:

- Connect the backend to the MySQL database.
- Perform CRUD (Create, Read, Update, Delete) operations.
- Store application data securely.
- Ensure reliable data communication.

---

# Technologies Used

- MySQL
- Node.js
- Express.js
- mysql2 Package
- dotenv

---

# Database Details

| Property | Value |
|----------|-------|
| Database Name | online_doctor_consultation |
| Database Type | MySQL |
| Port | 3306 |
| Host | localhost |

---

# Required Package

Install the MySQL package:

```bash
npm install mysql2
```

---

# Database Configuration (db.js)

```javascript
const mysql = require("mysql2");

const connection = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "your_password",
  database: "online_doctor_consultation"
});

connection.connect((err) => {
  if (err) {
    console.log("Database Connection Failed");
  } else {
    console.log("Database Connected Successfully");
  }
});

module.exports = connection;
```

---

# Database Tables

- Patients
- Doctors
- Appointments
- Admin

---

# Connection Flow

```
React Frontend
       │
       ▼
Express.js Backend
       │
       ▼
Database Connection (db.js)
       │
       ▼
MySQL Database
       │
       ▼
Store / Retrieve Data
```

---

# CRUD Operations

- Create new patient records
- Read doctor and appointment details
- Update user profiles
- Delete appointments (if required)

---

# Features

- Secure database connection
- Fast data retrieval
- Data storage and management
- CRUD operation support
- Error handling for connection failures

---

# Expected Output

- Backend successfully connects to MySQL.
- Data is stored and retrieved correctly.
- CRUD operations execute without errors.
- Connection status is displayed in the terminal.

---

# Future Enhancements

- Use Connection Pooling
- Environment Variables for Credentials
- Automatic Reconnection
- Database Backup Support
- Improved Error Logging

---

# Module Status

✔ MySQL Installed

✔ Database Created

✔ Connection Configured

✔ Backend Connected to Database

✔ CRUD Operations Enabled

✔ Database Connection Successfully Completed
