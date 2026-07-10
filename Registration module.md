# Registration Module

## Module Name
**Registration Module**

## Description

The Registration Module allows new patients and doctors to create an account in the Online Doctor Consultation System. The entered details are validated and securely stored in the MySQL database. After successful registration, users can log in using their registered email and password.

---

# Objective

The main objectives of the Registration Module are:

- Allow new users to create an account.
- Validate user information before submission.
- Store user details securely in the database.
- Prevent duplicate email registrations.
- Enable users to access the system after successful registration.

---

# User Roles

1. Patient
2. Doctor

---

# Registration Form Fields

## Patient Registration

| Field | Type | Required |
|--------|------|----------|
| Full Name | Text | Yes |
| Gender | Dropdown | Yes |
| Date of Birth | Date | Yes |
| Mobile Number | Number | Yes |
| Email | Email | Yes |
| Password | Password | Yes |
| Confirm Password | Password | Yes |
| Address | Textarea | Yes |

---

## Doctor Registration

| Field | Type | Required |
|--------|------|----------|
| Doctor Name | Text | Yes |
| Specialization | Text | Yes |
| Qualification | Text | Yes |
| Experience | Number | Yes |
| Mobile Number | Number | Yes |
| Email | Email | Yes |
| Password | Password | Yes |
| Hospital Name | Text | Yes |

---

# Validation Rules

- All mandatory fields must be filled.
- Email must be in a valid format.
- Mobile number must contain 10 digits.
- Password must be at least 8 characters.
- Password and Confirm Password must match.
- Email should not already exist.

---

# Registration Process

1. User opens the Registration page.
2. User selects Patient or Doctor.
3. User enters all required details.
4. React validates the form inputs.
5. User clicks the **Register** button.
6. Frontend sends data to the backend API.
7. Backend validates and stores the data in MySQL.
8. Registration success message is displayed.
9. User is redirected to the Login page.

---

# Registration Flow

```
User
   │
   ▼
Registration Form
   │
   ▼
React Frontend
   │
   ▼
Registration API
   │
   ▼
MySQL Database
   │
   ▼
Registration Successful
   │
   ▼
Login Page
```

---

# React Components

- Register.js
- Register.css
- ApiService.js

---

# Backend API

**POST /api/register**

### Request

```json
{
  "name": "John",
  "email": "john@example.com",
  "password": "password123",
  "mobile": "9876543210",
  "role": "Patient"
}
```

### Success Response

```json
{
  "message": "Registration Successful",
  "status": true
}
```

### Failure Response

```json
{
  "message": "Email already exists",
  "status": false
}
```

---

# Database Table

**patients**

- patient_id
- full_name
- gender
- date_of_birth
- mobile
- email
- password
- address

**doctors**

- doctor_id
- doctor_name
- specialization
- qualification
- experience
- mobile
- email
- password
- hospital_name

---

# Security Features

- Password validation
- Duplicate email checking
- Input validation
- Secure database storage

---

# Expected Output

- New user account created successfully.
- Registration details stored in the database.
- User redirected to the Login page.
- Error message shown for invalid or duplicate data.

---

# Module Status

✔ Registration Page Created

✔ Form Validation Completed

✔ API Connected

✔ Database Integration Completed

✔ Registration Successful

✔ Ready for Login
