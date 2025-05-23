# 🎵 MoodSphere – Emotion-Based Music Recommendation

**Capstone Project • Pace University (Spring 2024)**  
**Engineer:** Shane Parmar

---

## 🌟 Overview

MoodSphere is an AI-powered music recommendation system that curates personalized playlists based on the user's emotional state. Unlike traditional music recommenders that rely solely on genre or artist preferences, MoodSphere uses deep learning to detect facial expressions and recommend songs that reflect how the user feels in real time.

---

## 🚀 Features

- 🎭 Detects emotions using CNN + ResNet50 model from uploaded images
- 🎧 Suggests music based on detected mood
- 🔍 Search songs by **artist** and **genre**
- 🔐 Firebase Authentication (login/signup)
- 🧠 Personalized playlist management
- 🔌 RESTful API integrations with Flask backend
- 🖥️ Responsive frontend using React.js + Vite

---

## 🛠️ Tech Stack

| Layer      | Technology                       |
|------------|----------------------------------|
| Frontend   | React.js, Vite, JavaScript       |
| Backend    | Flask, Python, Firebase Admin SDK|
| ML Model   | CNN, ResNet50, TensorFlow        |
| Database   | Firebase Realtime DB             |
| Dev Tools  | GitHub, VS Code, Postman         |

---

## 🔄 API Endpoints

| Method | Endpoint             | Description                        |
|--------|----------------------|------------------------------------|
| POST   | `/predict`           | Predict mood from uploaded image   |
| POST   | `/songs-by-genre`    | Get songs matching a genre         |
| POST   | `/songs-by-artist`   | Get songs matching an artist       |
| GET    | `/get-playlist`      | Retrieve user playlist             |
| POST   | `/save-user`         | Save new user details              |

---

## 🧪 Running the Project Locally

### 🔧 Backend (Flask + TensorFlow)

```bash
cd moodsphere-backend
python -m venv venv
venv\Scripts\activate       # on Windows
pip install -r requirements.txt
python main.py              # Runs on http://127.0.0.1:5000

### 💻 Frontend (React)
bash
Copy
Edit
cd moodsphere
npm install
npm run dev                 # Runs on http://localhost:5173
