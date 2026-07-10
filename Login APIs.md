# Login APIs

## Module Name
**Login APIs**

## Description

The Login APIs module handles user authentication in the Online Doctor Consultation System. It verifies the user's email, password, and role before granting access to the application.

---

# Objective

The objectives of the Login APIs module are:

- Authenticate users securely.
- Validate login credentials.
- Allow role-based access.
- Return appropriate responses for successful or failed login attempts.

---

# Technologies Used

- Node.js
- Express.js
- MySQL
- JSON
- REST API

---

# API Endpoint

### User Login

**POST /api/login**

---

# Request Body

```json
{
  "email": "john@example.com",
  "password": "password123",
  "role": "Patient"
}
```

---

# Success Response

```json
{
  "status": true,
  "message": "Login Successful",
  "userId": 1,
  "role": "Patient"
}
```

---

# Failure Response

```json
{
  "status": false,
  "message": "Invalid Email or Password"
}
```

---

# Login Process

1. User enters Email, Password, and Role.
2. React frontend sends a POST request to the Login API.
3. Backend validates the user credentials.
4. Database checks whether the user exists.
5. If credentials are correct, login is successful.
6. User is redirected to the appropriate dashboard.
7. If credentials are incorrect, an error message is returned.

---

# Login Flow

```
User
   │
   ▼
Login Page
   │
   ▼
POST /api/login
   │
   ▼
Express.js Server
   │
   ▼
MySQL Database
   │
   ▼
Authentication
   │
   ├── Success → Dashboard
   │
   └── Failure → Error Message
```

---

# API Features

- Secure user authentication
- Role-based login
- Email validation
- Password verification
- JSON response
- Error handling

---

# Expected Output

- Valid users can log in successfully.
- Invalid credentials display an error message.
- Users are redirected to their respective dashboards.
- Authentication is completed securely.

---

# Future Enhancements

- JWT Authentication
- Password Encryption using bcrypt
- Multi-Factor Authentication (MFA)
- Forgot Password Feature
- Login Activity Logs

---

# Module Status

✔ Login API Created

✔ User Authentication Implemented

✔ Database Validation Completed

✔ JSON Response Implemented

✔ Role-Based Login Enabled

✔ Login APIs Successfully Completed
