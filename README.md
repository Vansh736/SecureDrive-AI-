
🔐 SecureDrive-AI

AI-Powered Adaptive Authentication and Intrusion Detection System

SecureDrive-AI is a hybrid cybersecurity application that combines adaptive behavioral authentication, machine learning intrusion detection, and OTP-based step-up verification to secure cloud-based user access.

The system uses a Flutter-based Android application connected to a FastAPI backend integrated with a Hybrid Intrusion Detection Engine (Random Forest + Adaptive Behavioral Engine) for real-time anomaly detection and intelligent authentication.

---

🚀 Features

- ✅ Adaptive Behavioral Authentication
- ✅ AI-Based Intrusion Detection
- ✅ OTP-Based Step-Up Verification
- ✅ Real-Time Anomaly Detection
- ✅ Behavioral Time-Cluster Learning
- ✅ Night Login Protection (1 AM – 5 AM)
- ✅ Behavioral Insights Dashboard
- ✅ Hybrid Machine Learning Engine
- ✅ Secure Login Session Tracking
- ✅ Risk-Based Authentication System

---

🧠 How the System Works

1. User logs into the Android application
2. Flutter app sends login activity to FastAPI backend
3. Backend extracts behavioral features
4. Hybrid IDS analyzes login behavior
5. System classifies activity as:
   - Normal
   - Suspicious / Anomaly
6. If anomaly detected:
   - OTP verification is triggered
7. After successful OTP verification:
   - Behavior becomes trusted and added to adaptive history

---

🏗️ System Architecture

Flutter Android App
        ↓
FastAPI Backend Server
        ↓
Hybrid ML Intrusion Detection Engine
(Random Forest + Adaptive Behavioral Engine)
        ↓
SQLite Behavioral Database

---

🤖 Hybrid Intrusion Detection Engine

The project uses a hybrid AI-based security architecture:

1. Random Forest Model

Detects:

- Suspicious login activity
- Unusual behavior patterns
- Intrusion attempts

2. Adaptive Behavioral Engine

Learns:

- User login routines
- Time-of-day behavior clusters
- Trusted authentication patterns

The system uses cyclical time-based clustering to intelligently recognize recurring daily login behavior.

---

🔐 Adaptive Authentication Logic

Learning Phase

- First 5 sessions are used for behavioral learning
- No OTP enforced during training phase

Anomaly Detection

After learning:

- Similar login times → Allow
- Unusual login times → OTP Required
- Night logins (1 AM – 5 AM) → Always OTP

Adaptive Learning

After OTP verification:

- The verified login pattern becomes trusted
- Future nearby logins do not require OTP again

Example:

11:10 AM → OTP Triggered
OTP Verified → Pattern Learned

Next Day:
11:05 AM → Normal Login
11:12 AM → Normal Login

---

📱 Mobile Application

The Android application provides:

- Secure Login Interface
- OTP Verification Screen
- Behavioral Insights Dashboard
- Real-Time Security Alerts
- File Upload and Access
- Test Time Offset Simulation Mode

---

📊 Behavioral Insights

The app visualizes:

- Login hour clusters
- Safe login zones
- Suspicious sessions
- OTP-triggered anomalies
- Adaptive learning patterns

---

🛠️ Technology Stack

Component| Technology
Frontend| Flutter (Dart)
Backend| FastAPI (Python)
Machine Learning| Scikit-learn, Pandas
Database| SQLite
APIs| REST APIs
Version Control| Git & GitHub

---

🗄️ Database Integration

SQLite is used for:

- Login history storage
- Behavioral session tracking
- OTP audit logs
- Adaptive learning data
- Intrusion activity logs

---

🔒 Security Features

- Backend-authoritative authentication
- OTP verification for suspicious logins
- Critical action protection
- Behavioral anomaly detection
- Time-cluster adaptive learning
- Real-time intrusion alerts

---

🌍 SDG Goal Alignment

This project aligns with:

SDG 9 — Industry, Innovation and Infrastructure

The system contributes by:

- Enhancing cybersecurity infrastructure
- Improving intelligent authentication systems
- Promoting secure digital environments
- Using AI for safer cloud-based platforms

---

📂 Project Structure

SecureDrive-AI/
│
├── mobile_app/        # Flutter Android Application
├── backend/           # FastAPI Backend Server
├── models/            # ML Models & IDS Logic
├── database/          # SQLite Behavioral Database
├── logs/              # Security & OTP Logs
└── README.md

---

⚡ Future Improvements

- Device fingerprinting
- IP reputation analysis
- Geo-location anomaly detection
- Cloud deployment
- Multi-factor authentication
- Advanced threat intelligence integration

---

👨‍💻 Author

Vansh Tiwari
B.E. Computer Science Engineering
Chitkara University

---

📜 License

This project is intended for educational, research, and cybersecurity learning purposes.
