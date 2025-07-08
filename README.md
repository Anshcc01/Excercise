# 🧘 Yoga Fit App - SIH 2025 Project

## 📌 Overview

**Yoga Fit App** is a full-stack AI-powered web application developed for **Smart India Hackathon 2025**. It helps users perform yoga postures correctly using **live camera detection**, providing **real-time feedback** with visual cues (e.g., green signal for correct posture). The system uses **OpenCV** and pose detection models, integrated with a React-based frontend and backend.

---

## 🎯 Key Features

- 📷 **Live Camera Integration** for Yoga Pose Detection  
- ✅ **Real-time Visual Feedback** (Green for correct pose, Red for incorrect)
- 🧘‍♀️ Detection for multiple popular Yoga Asanas
- 📡 **React-based Frontend** with interactive UI
- 🔧 **Backend in React/Node.js** serving OpenCV pose evaluation logic
- 📈 Scope for adding tracking, voice assistance, and user progress

---

## 🧠 Tech Stack

### 🔹 Frontend:
- **React.js**
- **Webcam.js / MediaPipe integration**
- **Tailwind CSS / Material UI (if used)**

### 🔹 Backend:
- **Node.js with Express**
- **OpenCV (via Python/Node bridge or REST API)**
- **Socket.IO / REST APIs** for real-time feedback

---

## 📂 Folder Structure

```
yoga-fit-app/
├── client/                   # React Frontend
│   ├── src/
│   │   ├── components/       # UI components (Camera, Feedback Panel)
│   │   ├── App.js
│   │   └── index.js
│   └── public/
├── server/                   # Node.js Backend
│   ├── pose-detector.py      # Python OpenCV script for pose checking
│   ├── server.js             # Express backend
│   └── routes/
│       └── detection.js      # API route to handle pose feedback
├── README.md
└── package.json              # Combined package manager file (or split in client/server)
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/yoga-fit-app.git
cd yoga-fit-app
```

### 2. Setup and Run Backend
```bash
cd server
npm install
node server.js
# Or if using Python for OpenCV
# python pose-detector.py (run separately)
```

### 3. Setup and Run Frontend
```bash
cd ../client
npm install
npm start
```

---

## 📷 How It Works

1. User enables camera access from the browser.
2. React frontend streams video using webcam.
3. Frames are sent to backend via API/WebSocket.
4. Backend uses **OpenCV** to detect pose and calculate angles.
5. Based on accuracy, frontend shows:
   - ✅ **Green border/indicator**: Correct pose
   - ❌ **Red warning**: Incorrect posture, with hints

---

## 📈 Future Enhancements

- Add more yoga pose models
- Voice-guided feedback and timers
- Mobile responsiveness / PWA support
- User login and progress tracking

---

## 📢 Acknowledgements

- Smart India Hackathon 2025
- OpenCV and MediaPipe
- React and Node.js Communities
- Yoga Pose Reference Datasets

---

> 🚀 A step toward making fitness accessible, AI-driven, and user-friendly!
