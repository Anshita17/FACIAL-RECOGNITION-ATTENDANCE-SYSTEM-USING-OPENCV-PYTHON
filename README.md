# 🧠 Face Recognition-Based Attendance System  
## An AI-Powered Attendance System Using Python and OpenCV

---

## 📌 Project Overview

Manual attendance is time-consuming, prone to errors, and lacks real-time monitoring. This project presents a **Python-based AI attendance system** that:

- 🔎 Detects faces using **OpenCV Haar Cascade Classifier**  
- 🧹 Captures and stores face images for registered users  
- 📊 Trains a **K-Nearest Neighbors (KNN)** model for face recognition  
- 🚨 Marks attendance automatically in a CSV file  
- 💻 Provides a **web-based interface** with **Flask** to add users and view attendance  

This system is useful for educational institutes, offices, and organizations to automate and streamline attendance recording.

---

## 🎯 Objectives

- Automate attendance taking using face recognition  
- Reduce human intervention and errors  
- Maintain a secure and organized record of attendance  
- Demonstrate real-world application of OpenCV, ML, and Flask  

---

## 🏗️ System Architecture

Web Interface (Flask)  
⬇  
Face Image Capture (OpenCV)  
⬇  
Face Detection (Haar Cascade)  
⬇  
Face Recognition (KNN Model)  
⬇  
Attendance Logging (CSV File)  
⬇  
Attendance Display (Web Page)

---

## 🛠️ Technologies Used

### Programming
- Python 3.9+  

### Libraries & Frameworks
- OpenCV (`cv2`) – Face detection and image capture  
- scikit-learn – KNN model for face recognition  
- Flask – Web interface  
- Pandas – Attendance CSV management  
- Joblib – Model saving and loading  

### Frontend
- HTML, CSS, Bootstrap  
- Jinja2 Templates  

### Storage
- `static/faces/` – Stores user face images  
- `Attendance/` – Stores attendance CSV files  

---

## 💻 How to Use This Project

---

### 🟢 OPTION 1 — Run Locally (Full Attendance System)

#### 1. Clone the repository

```bash
git clone https://github.com/YourUsername/Face-Recognition-Attendance-System.git
cd Face-Recognition-Attendance-System

````

#### 2. Create virtual environment

**macOS / Linux**

```bash
python3 -m venv venv
source venv/bin/activate
```

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

#### 3. Install dependencies

```bash
pip install -r requirements.txt
```

#### 4. Run the Flask app

```bash
python app.py
```

#### 5. Open in browser

```
http://127.0.0.1:5000
```

---

### 🟢 OPTION 2 — Add a New User

* Go to the "Add New User" section on the home page
* Enter **name** and **ID**
* The system will capture **10 face images** automatically
* Model will train automatically and save for recognition

---

### 🟢 OPTION 3 — Take Attendance

* Click **Take Attendance** on the home page
* The system detects registered faces in real-time using the webcam
* Marks attendance in `Attendance/Attendance-MM_DD_YY.csv`
* Displays **Name, ID, Time** in the web interface

---

### 🤖 Features

* Real-time face detection and recognition
* Automatic attendance logging
* Web interface to **view attendance records**
* Add/Delete users dynamically
* CSV-based storage for easy export

#### 💬 Example

| S No | Name    | ID  | Time     |
| ---- | ------- | --- | -------- |
| 1    | Anshita | 101 | 09:15:32 |
| 2    | John    | 102 | 09:16:10 |

---

### ⚠️ Notes / Troubleshooting

* Ensure your webcam is connected and accessible
* If no trained model exists, add at least one user before taking attendance
* Avoid running `cv2.imshow` in headless servers; it may cause OpenCV exceptions

---

### 🔮 Future Improvements

* Use **Deep Learning (FaceNet, MTCNN)** for higher accuracy
* Add **multi-user simultaneous recognition**
* Integrate **email/SMS alerts** for absentees
* Web-based live dashboard with **attendance analytics**
* Support for **multiple classrooms / departments**

---

### 📁 Repository Structure

```
Face-Recognition-Attendance-System/
│
├── app.py                # Main Flask app and core logic
├── home.html             # Homepage template
├── listusers.html        # Template to view registered users
├── start.html            # Template for attendance capture (optional)
├── static/
│   └── faces/            # Stores user face images
├── Attendance/           # Stores CSV attendance logs
├── haarcascade_frontalface_default.xml
├── requirements.txt
└── README.md
```

---

### 📬 Contact

Anshita Priyadarshini
[anshita.m04@gmail.com](mailto:anshita.m04@gmail.com)

---

⭐ If you find this project useful, consider giving it a star!




