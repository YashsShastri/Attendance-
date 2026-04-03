# Smart Attendance System

This project is a secure and automated attendance system designed to reduce proxy attendance and improve reliability in classrooms. The system uses a combination of QR code scanning, face recognition, and location verification to ensure that only valid students can mark their attendance.

The idea behind this project is to solve the common issue of fake attendance in colleges where students mark attendance for others. By integrating multiple layers of verification, this system makes attendance more trustworthy and efficient.

---

## Features

- Role-based login system (Admin, Teacher, Student)
- QR code generation for each lecture (valid for limited time)
- Face recognition for identity verification
- Location checking to ensure student is present in class
- Timetable management for teachers
- Automatic attendance storage
- Excel report generation (daily/lecture-wise)

---

## Working

1. The teacher logs into the system and selects the subject or lecture.
2. A QR code is generated which is valid for around 10 minutes.
3. Students scan the QR code using their device.
4. After scanning:
   - The system captures the student's face
   - Matches it with the registered image in the database
   - Verifies the student's location
5. If all conditions are satisfied, attendance is marked successfully.
6. At the end of the day, attendance data can be exported as an Excel file.

---

## Technologies Used

Frontend:
- HTML
- CSS
- JavaScript

Backend:
- Node.js / Python (Flask or Django)

Database:
- MongoDB / MySQL

Libraries / Tools:
- OpenCV (for face detection)
- Face Recognition models (pre-trained or custom CNN)
- QR Code Generator libraries

Optional Hardware:
- ESP32 (for IoT-based extensions)

---

## Project Structure

attendance-system/
│
├── backend/        # Server-side logic
├── frontend/       # UI files
├── models/         # ML models for face recognition
├── database/       # DB configurations
├── assets/         # Images and static files
└── README.md

---

## Security

- QR code expires after fixed time (10 minutes)
- Face recognition prevents fake attendance
- Location restriction ensures physical presence
- Authentication system for all users

---

## Limitations

- Requires good camera quality for accurate face detection
- Internet connection needed for real-time verification
- Location accuracy depends on device GPS

---

## Future Improvements

- Mobile application version
- Live dashboard for attendance tracking
- Cloud deployment
- Notification system for students and teachers

---

## Author

Yash Shastri  
Computer Engineering Student  

---

## Note

This project is developed as part of an academic and practical solution to improve attendance systems in colleges. Further improvements can be made by integrating advanced AI models and better hardware support.
