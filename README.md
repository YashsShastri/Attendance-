### 📊 Report Generation
- Automatic Excel report generation
- Daily and overall attendance tracking

---

## 🛠 Tech Stack

| Layer        | Technology |
|-------------|-----------|
| Frontend     | HTML, CSS, JavaScript |
| Backend      | Node.js / Flask / Django |
| Database     | MongoDB / MySQL |
| AI Model     | FaceNet / OpenCV / Deep Learning |
| Optional HW  | ESP32 |

---

## 📂 Project Structure


attendance-system/
│── backend/ # API and server logic
│── frontend/ # UI code
│── models/ # AI/ML models
│── database/ # DB schema / config
│── assets/ # Images / static files
│── README.md


---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository
```bash
git clone https://github.com/your-username/attendance-system.git
cd attendance-system
2️⃣ Install Dependencies
npm install
# OR (Python)
pip install -r requirements.txt
3️⃣ Run Backend
npm start
# OR
python app.py
4️⃣ Open Frontend
Open index.html
OR run frontend server
🔄 System Workflow
Teacher logs in
Generates QR code
Student scans QR
System captures:
Face image
Location
AI verifies identity
Attendance stored in database
Excel report generated
🔒 Security Mechanisms
⏱ QR expiration (10 minutes)
🧠 Face recognition validation
📍 Location restriction
🔑 Secure login system
📈 Future Scope
Mobile app (Android/iOS)
Cloud deployment (AWS/GCP)
Real-time dashboard
Biometric hardware integration
👨‍💻 Author

Yash Shastri
Computer Engineering Student
AI | IoT | Computer Vision
