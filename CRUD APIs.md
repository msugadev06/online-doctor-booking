# CRUD APIs

## Module Name
**CRUD APIs**

## Description

The CRUD APIs module provides RESTful API endpoints to perform **Create, Read, Update, and Delete** operations for Patients, Doctors, Appointments, and Admin users in the Online Doctor Consultation System.

---

# Objective

The objectives of the CRUD APIs module are:

- Create new records.
- Retrieve existing records.
- Update existing records.
- Delete unnecessary records.
- Enable communication between the frontend and the database.

---

# Technologies Used

- Node.js
- Express.js
- MySQL
- REST API
- JSON

---

# CRUD Operations

## Create (POST)

Used to add new records.

### APIs

- POST /api/patients
- POST /api/doctors
- POST /api/appointments

---

## Read (GET)

Used to retrieve records.

### APIs

- GET /api/patients
- GET /api/doctors
- GET /api/appointments
- GET /api/patients/:id
- GET /api/doctors/:id
- GET /api/appointments/:id

---

## Update (PUT)

Used to modify existing records.

### APIs

- PUT /api/patients/:id
- PUT /api/doctors/:id
- PUT /api/appointments/:id

---

## Delete (DELETE)

Used to remove records.

### APIs

- DELETE /api/patients/:id
- DELETE /api/doctors/:id
- DELETE /api/appointments/:id

---

# CRUD Flow

```
React Frontend
       │
       ▼
REST API Request
       │
       ▼
Express.js Server
       │
       ▼
MySQL Database
       │
       ▼
Response to Frontend
```

---

# Sample API Request

### Create Patient

```json
POST /api/patients

{
  "fullName": "John",
  "email": "john@example.com",
  "mobile": "9876543210"
}
```

### Success Response

```json
{
  "message": "Patient Created Successfully",
  "status": true
}
```

---

# Features

- Create new records
- View records
- Update records
- Delete records
- JSON response format
- Error handling
- Database integration

---

# Expected Output

- New records are successfully created.
- Existing records are displayed correctly.
- Records can be updated without errors.
- Records can be deleted successfully.
- API responses are returned in JSON format.

---

# Future Enhancements

- JWT Authentication
- Role-Based Access Control
- Pagination
- Search and Filter APIs
- API Documentation using Swagger

---

# Module Status

✔ Create API Implemented

✔ Read API Implemented

✔ Update API Implemented

✔ Delete API Implemented

✔ MySQL Integration Completed

✔ CRUD APIs Successfully Completed
