# API Testing Report

## Module Name
**API Testing Report**

## Description

The API Testing Report verifies that all REST APIs in the Online Doctor Consultation System are functioning correctly. Testing ensures that each API returns the expected response and performs the required database operations successfully.

---

# Objective

The objectives of API testing are:

- Verify API functionality.
- Validate request and response data.
- Ensure proper database interaction.
- Identify and fix API errors.
- Confirm successful integration with the frontend.

---

# Testing Tools

- Postman
- Node.js
- Express.js
- MySQL

---

# APIs Tested

## 1. Login API

**Method:** POST

**Endpoint:**
```
/api/login
```

**Status:** ✅ Passed

---

## 2. Patient Registration API

**Method:** POST

**Endpoint:**
```
/api/patients
```

**Status:** ✅ Passed

---

## 3. Doctor Registration API

**Method:** POST

**Endpoint:**
```
/api/doctors
```

**Status:** ✅ Passed

---

## 4. View Doctors API

**Method:** GET

**Endpoint:**
```
/api/doctors
```

**Status:** ✅ Passed

---

## 5. Book Appointment API

**Method:** POST

**Endpoint:**
```
/api/appointments
```

**Status:** ✅ Passed

---

## 6. View Appointments API

**Method:** GET

**Endpoint:**
```
/api/appointments
```

**Status:** ✅ Passed

---

## 7. Update Appointment API

**Method:** PUT

**Endpoint:**
```
/api/appointments/:id
```

**Status:** ✅ Passed

---

## 8. Delete Appointment API

**Method:** DELETE

**Endpoint:**
```
/api/appointments/:id
```

**Status:** ✅ Passed

---

# Test Results

| API | Method | Result |
|------|--------|--------|
| Login | POST | Passed |
| Patient Registration | POST | Passed |
| Doctor Registration | POST | Passed |
| View Doctors | GET | Passed |
| Book Appointment | POST | Passed |
| View Appointments | GET | Passed |
| Update Appointment | PUT | Passed |
| Delete Appointment | DELETE | Passed |

---

# Response Format

Example Success Response:

```json
{
  "status": true,
  "message": "Request Successful"
}
```

Example Failure Response:

```json
{
  "status": false,
  "message": "Invalid Request"
}
```

---

# Testing Summary

- All APIs executed successfully.
- Database operations completed correctly.
- JSON responses received as expected.
- No major errors detected during testing.
- Frontend and backend communication verified.

---

# Future Improvements

- Automated API testing using Jest or Mocha.
- Performance and load testing.
- Security testing with JWT authentication.
- API documentation using Swagger.

---

# Module Status

✔ Login API Tested

✔ Patient API Tested

✔ Doctor API Tested

✔ Appointment API Tested

✔ CRUD APIs Tested

✔ Database Integration Verified

✔ API Testing Successfully Completed
