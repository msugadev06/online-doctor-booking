# Data Listing Module

## Module Name
**Data Listing Module**

## Description

The Data Listing Module displays information stored in the database in a structured and user-friendly format. It allows users to view, search, sort, and manage records such as doctors, patients, and appointments.

---

# Objective

The main objectives of the Data Listing Module are:

- Display records from the database.
- Provide quick access to important information.
- Allow searching and filtering of records.
- Improve data management and user experience.

---

# Data Lists Included

### 1. Doctor List

Displays:
- Doctor ID
- Doctor Name
- Specialization
- Qualification
- Experience
- Contact Number
- Availability

---

### 2. Patient List

Displays:
- Patient ID
- Patient Name
- Gender
- Age
- Mobile Number
- Email

---

### 3. Appointment List

Displays:
- Appointment ID
- Patient Name
- Doctor Name
- Appointment Date
- Appointment Time
- Consultation Type
- Status

---

### 4. Consultation History

Displays:
- Consultation ID
- Patient Name
- Doctor Name
- Consultation Date
- Diagnosis
- Prescription

---

# Features

- View all records
- Search records
- Filter data
- Sort records
- Pagination support
- Update records
- Delete records (Admin only)

---

# Data Listing Flow

```
Database
   │
   ▼
Backend API
   │
   ▼
React Components
   │
   ▼
Display Records
   │
   ▼
Search / Filter / Sort
```

---

# React Components

- DoctorList.js
- PatientList.js
- AppointmentList.js
- ConsultationHistory.js

---

# Backend APIs

**GET /api/doctors**

Returns all registered doctors.

---

**GET /api/patients**

Returns all registered patients.

---

**GET /api/appointments**

Returns all booked appointments.

---

**GET /api/consultations**

Returns consultation history.

---

# Expected Output

- Doctors displayed in a table.
- Patients displayed in a table.
- Appointments displayed with status.
- Consultation history available for authorized users.
- Search and filter options work correctly.

---

# Module Status

✔ Doctor Listing Completed

✔ Patient Listing Completed

✔ Appointment Listing Completed

✔ Consultation History Added

✔ Search Functionality Implemented

✔ Filter and Sorting Implemented

✔ Backend API Connected

✔ Data Listing Module Successfully Completed
