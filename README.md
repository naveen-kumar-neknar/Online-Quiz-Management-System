# 🧠 Online Quiz Management System

A full-stack web application that allows users to take quizzes, store results, and manage user data. The system uses a modern React frontend and a Node.js backend with MongoDB for data storage.

---

## 🚀 Features

* 👤 User Registration and Login
* 📝 Attempt Quizzes
* 📊 Store and View Results
* 🔗 Results linked with User ID
* 🗄️ MongoDB Database Integration
* ⚡ Fast and responsive UI using Vite

---

## 🛠️ Tech Stack

### Frontend

* React (Vite)
* JavaScript
* CSS

### Backend

* Node.js
* Express.js

### Database

* MongoDB (Compass / Atlas)
* Mongoose

---

## 📂 Project Structure

```
Online-Quiz-Management-System/
│
├── frontend/               # React frontend (Vite)
│   ├── src/
│   ├── components/
│   ├── pages/
│   └── package.json
│
├── backend/                # Node.js backend
│   ├── config/             # Database connection
│   ├── models/             # Mongoose models (User, Result)
│   ├── routes/             # API routes
│   ├── server.js
│   └── package.json
│
├── .gitignore
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone Repository

```
git clone https://github.com/naveen-kumar-neknar/Online-Quiz-Management-System.git
cd Online-Quiz-Management-System
```

---

## ▶️ Run Backend

```
cd backend
npm install
npm run dev
```

Backend runs on:

```
http://localhost:5000
```

---

## ▶️ Run Frontend

Open another terminal:

```
cd frontend
npm install
npm run dev
```

Frontend runs on:

```
http://localhost:5173
```

---

## 🔧 Environment Variables

Create a `.env` file inside `backend/` folder:

```
MONGO_URI=mongodb://127.0.0.1:27017/quiz-app
PORT=5000
```

---

## 🗄️ Database

* MongoDB stores:

  * Users
  * Quiz Results

* Each result is linked with a user using:

```
userId
```

---

## 🌐 API Example

### Save Quiz Result

POST `/api/results`

```
{
  "userId": "USER_ID_HERE",
  "score": 8,
  "totalQuestions": 10
}
```

---

## 🚀 Deployment

### Backend (Render)

* Root Directory: backend
* Build Command: npm install
* Start Command: npm run dev

### Frontend (Vercel)

* Root Directory: frontend
* Framework: Vite

---

## ⚠️ Important Notes

* Do NOT upload `node_modules`
* Use `.gitignore`:

```
node_modules/
.env
```

* Ensure backend uses:

```
const PORT = process.env.PORT || 5000;
```

* Enable CORS in backend if needed

---

## 👨‍💻 Author

Developed by Neknar Naveen Kumar



---
