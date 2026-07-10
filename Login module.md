# Login Module

## Module Name
**Login Module**

## Description

The Login Module allows Patients, Doctors, and Administrators to securely access the Online Doctor Consultation System using their registered email and password. After successful authentication, users are redirected to their respective dashboards.

---

# Objective

The main objective of the Login Module is to:

- Provide secure user authentication.
- Verify user credentials.
- Allow role-based access (Patient, Doctor, Admin).
- Protect unauthorized access to the system.

---

# User Roles

1. Patient
2. Doctor
3. Administrator

---

# Login Form Fields

| Field | Type | Required |
|--------|------|----------|
| Email | Email | Yes |
| Password | Password | Yes |
| User Role | Dropdown | Yes |

---

# Validation Rules

- Email should be in valid format.
- Password cannot be empty.
- User role must be selected.
- Invalid credentials display an error message.

---

# Login Process

1. User opens the Login page.
2. User enters Email.
3. User enters Password.
4. User selects Role.
5. Clicks **Login** button.
6. React sends the request to the backend API.
7. Backend validates the credentials using the database.
8. If valid, the user is redirected to the respective dashboard.
9. If invalid, an error message is displayed.

---

# Login Flow

```
User
   │
   ▼
Login Form
   │
   ▼
React Frontend
   │
   ▼
Login API
   │
   ▼
MySQL Database
   │
   ▼
Authentication Successful
   │
   ▼
Dashboard
```

---

# React Components

- Login.js
- Login.css
- ApiService.js

---

# Backend API

**POST /api/login**

### Request

```json
{
  "email": "patient@example.com",
  "password": "password123",
  "role": "Patient"
}
```

### Success Response

```json
{
  "message": "Login Successful",
  "status": true
}
```

### Failure Response

```json
{
  "message": "Invalid Email or Password",
  "status": false
}
```

---

# Security Features

- Password validation
- Session management
- Role-based authentication
- Protected routes
- Logout functionality

---

# Expected Output

- Patient Dashboard after patient login.
- Doctor Dashboard after doctor login.
- Admin Dashboard after admin login.
- Error message for invalid credentials.

---

# Module Status

✔ Login Page Created

✔ Form Validation Completed

✔ API Connected

✔ Authentication Implemented

✔ Dashboard Redirection Completed

✔ Login Module Successfully Implemented
