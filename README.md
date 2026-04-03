# Smart Attendance System

## Introduction

This project presents a secure and automated attendance system designed for academic institutions. The system combines QR code-based attendance with face recognition and location verification to ensure that attendance is marked only by authorized students physically present in the classroom.

The main objective is to eliminate proxy attendance and manual errors while keeping the process simple for both teachers and students.

---

## Objectives

- Reduce proxy attendance
- Automate attendance marking process
- Ensure identity verification using face recognition
- Validate physical presence using location tracking
- Generate structured attendance reports

---

## System Overview

| Module            | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| Authentication    | Login system for Admin, Teacher, and Student                                |
| QR Generator      | Generates time-limited QR codes for each lecture                            |
| Face Recognition  | Verifies student identity using stored facial data                          |
| Location Check    | Ensures student is within classroom boundary                                |
| Attendance Logic  | Marks attendance after all validations                                      |
| Report System     | Generates Excel reports of attendance                                       |

---

## Features

| Feature                     | Details                                                                 |
|----------------------------|-------------------------------------------------------------------------|
| Role-based Access          | Separate dashboards for Admin, Teacher, and Student                     |
| QR Code Attendance         | QR valid for limited duration (approx. 10 minutes)                      |
| Face Verification          | Matches captured image with registered student data                     |
| Location Validation        | Uses GPS to verify presence                                             |
| Timetable Management       | Teachers can manage lecture schedules                                   |
| Data Storage               | Attendance stored in database                                           |
| Report Generation          | Export attendance in Excel format                                       |

---

## Working Process

1. Teacher logs into the system.
2. Selects subject and lecture.
3. Generates a QR code for that session.
4. Students scan the QR code.
5. System performs:
   - Face capture and matching
   - Location verification
6. If all checks pass, attendance is recorded.
7. Data is stored and can be exported later.

---

## Technology Stack

### Frontend

| Technology | Purpose                     |
|------------|-----------------------------|
| HTML       | Structure of web pages      |
| CSS        | Styling                     |
| JavaScript | Client-side functionality   |

### Backend

| Technology          | Purpose                        |
|--------------------|--------------------------------|
| Node.js / Python   | Server-side logic              |
| Flask / Django     | API handling (if Python used)  |

### Database

| Database  | Usage                  |
|-----------|------------------------|
| MongoDB   | NoSQL data storage     |
| MySQL     | Relational storage     |

### Libraries and Tools

| Tool / Library | Purpose                              |
|----------------|--------------------------------------|
| OpenCV         | Face detection                       |
| FaceNet / CNN  | Face recognition                     |
| QR Libraries   | QR code generation                   |

---

## Project Structure
attendance-system/
│
├── backend/ # API and server logic
├── frontend/ # UI components
├── models/ # Face recognition models
├── database/ # DB setup and schemas
├── assets/ # Static files
└── README.md


---

## Security Measures

| Security Layer     | Description                                      |
|-------------------|--------------------------------------------------|
| QR Expiry         | QR code valid for limited time only              |
| Face Matching     | Prevents unauthorized users                      |
| Location Check    | Restricts attendance to classroom area           |
| Authentication    | Secure login system for all users                |

---

## Limitations

- Face recognition accuracy depends on lighting and camera quality
- GPS accuracy may vary depending on device
- Requires internet connectivity for real-time validation

---

## Future Scope

| Improvement Area        | Description                                      |
|------------------------|--------------------------------------------------|
| Mobile Application     | Dedicated Android/iOS app                        |
| Cloud Deployment       | Hosting system on cloud                          |
| Analytics Dashboard    | Attendance insights and statistics               |
| Notification System    | Alerts for attendance status                     |

---

## Author

Yash Shastri  
Computer Engineering Student  

---

## Conclusion

This system provides a practical and scalable solution to modern attendance problems. By combining multiple verification methods, it ensures reliability and reduces manual intervention. The project can be further enhanced with advanced AI models and deployment strategies.







