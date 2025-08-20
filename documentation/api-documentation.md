# API Endpoints and Webhooks

## Overview

This document contains details for the custom API endpoints (webhooks) used to communicate between Vapi AI assistant and Make.com workflows.

## Webhooks

### 1. Check Availability

- **URL:** Provided by Make.com webhook module  
- **Method:** POST  
- **Request Body Example:**

{
"preferred_date": "2025-08-10",
"preferred_time": "14:00",
"doctor_name": "Dr. Smith",
"appointment_duration": 30
}

- **Response Example:**

{
"available": true
}

### 2. Book Appointment

- **URL:** Provided by Make.com webhook module  
- **Method:** POST  
- **Request Body Example:**

{
"patient_name": "John Doe",
"phone_number": "+1234567890",
"email": "john.doe@example.com",
"appointment_date": "2025-08-10",
"appointment_time": "14:00",
"doctor_name": "Dr. Smith",
"chief_complaint": "Routine checkup",
"duration_minutes": 30
}

- **Response Example:**

{
"success": true,
"message": "Appointment booked successfully!"
}

text
undefined
