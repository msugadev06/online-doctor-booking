# Forms Module

## Module Name
**Forms Module**

## Description

The Forms Module is responsible for collecting and validating user information in the Online Doctor Consultation System. It provides user-friendly forms for registration, login, appointment booking, profile management, and other system operations.

---

# Objective

The main objectives of the Forms Module are:

- Collect user information accurately.
- Validate input before submission.
- Reduce data entry errors.
- Improve user experience.
- Send valid data to the backend database.

---

# Forms Included

### 1. Patient Registration Form
Fields:
- Full Name
- Gender
- Date of Birth
- Mobile Number
- Email
- Password
- Confirm Password
- Address

---

### 2. Doctor Registration Form
Fields:
- Doctor Name
- Specialization
- Qualification
- Experience
- Mobile Number
- Email
- Password
- Hospital Name

---

### 3. Login Form
Fields:
- Email
- Password
- User Role

---

### 4. Appointment Booking Form
Fields:
- Patient Name
- Doctor Name
- Specialization
- Appointment Date
- Appointment Time
- Consultation Type
- Symptoms

---

### 5. Patient Profile Form
Fields:
- Name
- Mobile Number
- Email
- Address
- Date of Birth

---

### 6. Doctor Profile Form
Fields:
- Doctor Name
- Qualification
- Specialization
- Experience
- Hospital Name
- Contact Number

---

# Form Validation

- All required fields must be filled.
- Email must be in a valid format.
- Mobile number must contain 10 digits.
- Password must be at least 8 characters.
- Password and Confirm Password must match.
- Appointment date cannot be in the past.
- Invalid data displays an error message.

---

# Form Submission Process

```
User
   │
   ▼
Fill Form
   │
   ▼
Input Validation
   │
   ▼
Submit Form
   │
   ▼
Backend API
   │
   ▼
MySQL Database
   │
   ▼
Success Message
```

---

# React Components

- Login.js
- Register.js
- AppointmentForm.js
- PatientProfile.js
- DoctorProfile.js

---

# Features

- Responsive Design
- Real-Time Validation
- Error Messages
- Required Field Validation
- Secure Data Submission
- Easy Navigation

---

# Expected Output

- Users can successfully submit forms.
- Valid data is stored in the database.
- Invalid entries are rejected with proper messages.
- Users receive confirmation after successful submission.

---

# Module Status

✔ Patient Registration Form Completed

✔ Doctor Registration Form Completed

✔ Login Form Completed

✔ Appointment Booking Form Completed

✔ Patient Profile Form Completed

✔ Doctor Profile Form Completed

✔ Form Validation Implemented

✔ Backend Integration Completed

✔ Forms Module Successfully Completed
