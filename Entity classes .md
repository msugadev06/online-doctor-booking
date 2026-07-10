# Entity Classes

## Module Name
**Entity Classes**

## Description

Entity classes represent the main objects in the Online Doctor Consultation System. Each entity corresponds to a table in the MySQL database and stores information related to patients, doctors, appointments, and administrators.

---

# Objective

The objectives of the Entity Classes module are:

- Represent database tables as objects.
- Store application data in a structured format.
- Simplify database operations.
- Support CRUD (Create, Read, Update, Delete) functionality.

---

# Entities

## 1. Patient Entity

### Attributes

| Field | Data Type |
|--------|-----------|
| patientId | Integer |
| fullName | String |
| gender | String |
| dateOfBirth | Date |
| mobile | String |
| email | String |
| password | String |
| address | String |

---

## 2. Doctor Entity

### Attributes

| Field | Data Type |
|--------|-----------|
| doctorId | Integer |
| doctorName | String |
| specialization | String |
| qualification | String |
| experience | Integer |
| mobile | String |
| email | String |
| password | String |
| hospitalName | String |

---

## 3. Appointment Entity

### Attributes

| Field | Data Type |
|--------|-----------|
| appointmentId | Integer |
| patientId | Integer |
| doctorId | Integer |
| appointmentDate | Date |
| appointmentTime | Time |
| consultationType | String |
| symptoms | String |
| status | String |

---

## 4. Admin Entity

### Attributes

| Field | Data Type |
|--------|-----------|
| adminId | Integer |
| adminName | String |
| email | String |
| password | String |

---

# Entity Relationships

- One Patient can book many Appointments.
- One Doctor can attend many Appointments.
- Each Appointment belongs to one Patient and one Doctor.
- Admin manages Patients, Doctors, and Appointments.

---

# Entity Flow

```
Patient
    │
    ▼
Appointment
    ▲
    │
Doctor

       ▲
       │
     Admin
```

---

# Benefits

- Structured data management
- Easy database mapping
- Better code organization
- Simplified CRUD operations
- Improved maintainability

---

# Expected Output

- Patient details stored correctly.
- Doctor details stored correctly.
- Appointment information linked with patients and doctors.
- Admin manages all system data efficiently.

---

# Module Status

✔ Patient Entity Created

✔ Doctor Entity Created

✔ Appointment Entity Created

✔ Admin Entity Created

✔ Entity Relationships Defined

✔ Entity Classes Successfully Completed
