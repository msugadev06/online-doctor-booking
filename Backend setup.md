# Backend Setup

## Module Name
**Backend Setup**

## Description

The Backend of the Online Doctor Consultation System is responsible for handling business logic, processing client requests, communicating with the MySQL database, and providing secure REST APIs for the frontend.

---

# Objective

The main objectives of the Backend Setup are:

- Develop RESTful APIs.
- Connect the application with the MySQL database.
- Handle user authentication and authorization.
- Manage patient, doctor, and appointment data.
- Ensure secure and reliable data processing.

---

# Technologies Used

- Node.js
- Express.js
- MySQL
- CORS
- dotenv
- Nodemon

---

# Software Requirements

- Node.js (Latest LTS Version)
- npm
- Visual Studio Code
- MySQL Server
- Git

---

# Backend Project Setup

## Step 1: Create Backend Folder

```bash
mkdir backend
cd backend
```

---

## Step 2: Initialize Node.js Project

```bash
npm init -y
```

---

## Step 3: Install Required Packages

```bash
npm install express mysql2 cors dotenv
npm install --save-dev nodemon
```

---

# Recommended Folder Structure

```
backend/
│
├── config/
│   └── db.js
│
├── controllers/
│   ├── authController.js
│   ├── doctorController.js
│   ├── patientController.js
│   └── appointmentController.js
│
├── routes/
│   ├── authRoutes.js
│   ├── doctorRoutes.js
│   ├── patientRoutes.js
│   └── appointmentRoutes.js
│
├── models/
│   ├── Doctor.js
│   ├── Patient.js
│   └── Appointment.js
│
├── server.js
├── package.json
└── .env
```

---

# Backend Features

- User Authentication
- Patient Management
- Doctor Management
- Appointment Booking
- Appointment Cancellation
- Profile Management
- REST API Support

---

# API Modules

- Authentication API
- Patient API
- Doctor API
- Appointment API
- Admin API

---

# Database Connectivity

The backend connects to the MySQL database using the **mysql2** package. All CRUD operations are performed through secure database queries.

---

# Running the Backend Server

Start the development server using:

```bash
npm run dev
```

Or start normally using:

```bash
node server.js
```

Server runs at:

```
http://localhost:5000
```

---

# Expected Output

- Backend server starts successfully.
- Database connection is established.
- APIs are available for frontend requests.
- User authentication and data management work correctly.

---

# Future Enhancements

- JWT Authentication
- Password Encryption (bcrypt)
- Email Notifications
- File Upload Support
- Video Consultation API
- Online Payment Integration

---

# Module Status

✔ Backend Project Created

✔ Express Server Configured

✔ Required Packages Installed

✔ MySQL Connected

✔ API Routes Created

✔ Environment Variables Configured

✔ Backend Ready for Development
