# 🧠 Online Quiz Management System

> A full-stack web application that allows users to register, log in, attempt quizzes, store quiz results, and manage user data using a modern **React + Vite frontend**, **Node.js + Express backend**, and **MongoDB database**.

![React](https://img.shields.io/badge/Frontend-React-61DAFB?logo=react)
![Vite](https://img.shields.io/badge/Build-Vite-646CFF?logo=vite)
![JavaScript](https://img.shields.io/badge/Language-JavaScript-F7DF1E?logo=javascript)
![Node.js](https://img.shields.io/badge/Backend-Node.js-339933?logo=node.js)
![Express](https://img.shields.io/badge/Framework-Express-black?logo=express)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-47A248?logo=mongodb)
![Mongoose](https://img.shields.io/badge/ODM-Mongoose-880000)

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [Key Features](#-key-features)
- [Use Cases](#-use-cases)
- [Technology Stack](#-technology-stack)
- [System Workflow](#-system-workflow)
- [System Architecture](#-system-architecture)
- [Project Structure](#-project-structure)
- [Requirements](#-requirements)
- [Installation and Setup](#-installation-and-setup)
- [Backend Setup](#-backend-setup)
- [Frontend Setup](#-frontend-setup)
- [Environment Variables](#-environment-variables)
- [Database](#-database)
- [API Example](#-api-example)
- [Running the Application](#-running-the-application)
- [Deployment](#-deployment)
- [Important Notes](#-important-notes)
- [Troubleshooting](#-troubleshooting)
- [Future Scope](#-future-scope)
- [Contribution](#-contribution)
- [Author](#-author)
- [License](#-license)

---

# 🚀 Project Overview

The **Online Quiz Management System** is a full-stack web application designed to provide an interactive platform for users to take quizzes and manage their quiz results.

The application consists of a React frontend, Node.js backend, and MongoDB database.

The system allows users to:

- Register and log in.
- Attempt quizzes.
- Submit quiz results.
- Store quiz scores.
- View previous results.
- Associate results with the corresponding user.

The overall application architecture is:

```text
React Frontend
       ↓
Node.js + Express Backend
       ↓
Mongoose
       ↓
MongoDB
```

---

# 🎯 Objectives

The main objectives of the project are:

1. Provide a web-based platform for taking quizzes.
2. Allow users to register and log in.
3. Allow users to attempt quizzes.
4. Store quiz results in MongoDB.
5. Associate quiz results with the corresponding user.
6. Allow users to view their quiz results.
7. Provide a fast and responsive user interface.
8. Build the application using a full-stack architecture.

---

# ✨ Key Features

## 👤 User Registration and Login

Users can create an account and log in to access the quiz system.

---

## 📝 Attempt Quizzes

Registered users can attempt available quizzes through the frontend application.

---

## 📊 Store and View Results

Quiz results are stored in MongoDB and can be viewed by users.

---

## 🔗 Results Linked with User ID

Each quiz result is associated with the user who attempted the quiz.

The relationship is maintained using:

```text
userId
```

---

## 🗄️ MongoDB Database Integration

MongoDB is used to store application data.

Mongoose is used to interact with MongoDB from the Node.js backend.

---

## ⚡ Fast and Responsive UI

The frontend is built using **React with Vite**, providing a fast development and responsive application experience.

---

# 👨‍💻 Use Cases

## 📝 Online Quiz Platform

Users can take quizzes through the web application.

## 👤 User Management

Users can register and log in to the system.

## 📊 Result Management

Quiz scores and result information can be stored and accessed.

## 🔗 User-Specific Results

Each result is associated with the corresponding user's `userId`.

## 🗄️ Centralized Data Storage

MongoDB provides persistent storage for users and quiz results.

---

# 🧰 Technology Stack

| Category | Technology |
|---|---|
| Frontend | React |
| Frontend Build Tool | Vite |
| Programming Language | JavaScript |
| Styling | CSS |
| Backend | Node.js |
| Backend Framework | Express.js |
| Database | MongoDB |
| Database ODM | Mongoose |
| Database Tools | MongoDB Compass / MongoDB Atlas |
| Version Control | Git / GitHub |

---

# 🔄 System Workflow

The application follows this basic workflow:

```text
User
 ↓
Register / Login
 ↓
Access Quiz
 ↓
Attempt Quiz
 ↓
Submit Answers
 ↓
Calculate Score
 ↓
Save Result
 ↓
Link Result with User ID
 ↓
MongoDB
 ↓
View Results
```

---

# 🏗️ System Architecture

```text
                         USER
                           │
                           ▼
                 ┌──────────────────┐
                 │  React Frontend  │
                 │      + Vite      │
                 └────────┬─────────┘
                          │
                          ▼
                 ┌──────────────────┐
                 │ Node.js +        │
                 │ Express Backend  │
                 └────────┬─────────┘
                          │
                          ▼
                    ┌───────────┐
                    │ Mongoose  │
                    └─────┬─────┘
                          │
                          ▼
                 ┌──────────────────┐
                 │     MongoDB      │
                 │                  │
                 │ Users            │
                 │ Quiz Results     │
                 └──────────────────┘
```

---

# 📁 Project Structure

```text
Online-Quiz-Management-System/
│
├── frontend/                  # React frontend (Vite)
│   │
│   ├── src/
│   │
│   ├── components/
│   │
│   ├── pages/
│   │
│   └── package.json
│
├── backend/                   # Node.js backend
│   │
│   ├── config/               # Database connection
│   │
│   ├── models/               # Mongoose models
│   │   ├── User
│   │   └── Result
│   │
│   ├── routes/               # API routes
│   │
│   ├── server.js
│   │
│   └── package.json
│
├── .gitignore
│
└── README.md
```

---

# 💻 Requirements

Before running the project, make sure the following are installed:

- Node.js
- npm
- MongoDB
- Git

The project can use either:

```text
MongoDB Compass
```

or:

```text
MongoDB Atlas
```

for database management/storage.

---

# ⚙️ Installation and Setup

First, clone the repository:

```bash
git clone https://github.com/naveen-kumar-neknar/Online-Quiz-Management-System.git
```

Navigate into the project:

```bash
cd Online-Quiz-Management-System
```

The frontend and backend must then be configured separately.

---

# ⚙️ Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Install the required dependencies:

```bash
npm install
```

Create the environment configuration file as described in the [Environment Variables](#-environment-variables) section.

Start the backend in development mode:

```bash
npm run dev
```

The backend runs on:

```text
http://localhost:5000
```

---

# 🌐 Frontend Setup

Open another terminal.

Navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the Vite development server:

```bash
npm run dev
```

The frontend runs on:

```text
http://localhost:5173
```

---

# 🔐 Environment Variables

Create a `.env` file inside:

```text
backend/
```

Add:

```env
MONGO_URI=mongodb://127.0.0.1:27017/quiz-app
PORT=5000
```

### Environment Variables

| Variable | Purpose |
|---|---|
| `MONGO_URI` | MongoDB database connection string |
| `PORT` | Backend server port |

For MongoDB Atlas, replace the local MongoDB connection string with your MongoDB Atlas connection string.

---

# 🗄️ Database

The application uses **MongoDB** for persistent data storage.

MongoDB stores:

```text
Users
Quiz Results
```

The backend uses **Mongoose** to define and interact with the MongoDB data models.

---

## 🔗 Result and User Relationship

Each quiz result is associated with a user through:

```text
userId
```

This allows the system to associate each result with the corresponding user.

Example:

```text
User
 │
 └── userId
       │
       ▼
   Quiz Result
       │
       ├── score
       └── totalQuestions
```

---

# 🌐 API Example

## Save Quiz Result

### Endpoint

```text
POST /api/results
```

### Request Body

```json
{
  "userId": "USER_ID_HERE",
  "score": 8,
  "totalQuestions": 10
}
```

The result contains:

| Field | Description |
|---|---|
| `userId` | ID of the user who attempted the quiz |
| `score` | Score obtained by the user |
| `totalQuestions` | Total number of questions |

---

# ▶️ Running the Application

The complete application requires both the backend and frontend to run.

## Terminal 1 — Backend

```bash
cd backend
npm install
npm run dev
```

Backend:

```text
http://localhost:5000
```

---

## Terminal 2 — Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend:

```text
http://localhost:5173
```

---

# 🔄 Complete End-to-End Workflow

```text
User Opens Application
        ↓
React + Vite Frontend
        ↓
Register / Login
        ↓
Attempt Quiz
        ↓
Submit Quiz
        ↓
Backend API
        ↓
Calculate / Receive Result
        ↓
Associate Result with userId
        ↓
Mongoose
        ↓
MongoDB
        ↓
Store Quiz Result
        ↓
User Views Result
```

---

# 🚀 Deployment

## Backend — Render

The backend can be deployed using **Render**.

### Configuration

```text
Root Directory:
backend
```

### Build Command

```bash
npm install
```

### Start Command

```bash
npm run dev
```

---

## Frontend — Vercel

The frontend can be deployed using **Vercel**.

### Configuration

```text
Root Directory:
frontend
```

### Framework

```text
Vite
```

---

# ⚠️ Important Notes

## Do Not Upload `node_modules`

Do not commit dependency folders to GitHub.

Use:

```text
node_modules/
```

inside `.gitignore`.

---

## Do Not Upload `.env`

The `.env` file should not be committed because it contains database configuration.

Use:

```text
.env
```

inside `.gitignore`.

---

## Recommended `.gitignore`

```text
node_modules/
.env
```

---

## Backend Port

Make sure the backend uses the configured environment port:

```javascript
const PORT = process.env.PORT || 5000;
```

---

## CORS

Enable CORS in the backend if the frontend and backend are running on different origins.

---

# 🛠️ Troubleshooting

## Backend Does Not Start

Check that:

```text
Node.js is installed
npm install has been completed
.env exists
MongoDB connection is configured
```

Then run:

```bash
npm run dev
```

---

## MongoDB Connection Error

Check:

```text
MONGO_URI
MongoDB server / Atlas connection
Database availability
```

For local MongoDB, the configured connection is:

```text
mongodb://127.0.0.1:27017/quiz-app
```

---

## Frontend Does Not Start

Run:

```bash
npm install
```

Then:

```bash
npm run dev
```

The Vite development server should be available at:

```text
http://localhost:5173
```

---

## Frontend Cannot Connect to Backend

Verify that the backend is running on:

```text
http://localhost:5000
```

Also make sure CORS is configured correctly if required.

---

# 🚧 Future Scope

Future improvements can include:

- Additional quiz categories.
- More quiz management functionality.
- Enhanced result analytics.
- Additional user features.
- Improved quiz administration functionality.

---

# 🤝 Contribution

Contributions are welcome.

For major changes, please open an issue first to discuss the proposed changes.

---

# 👨‍💻 Author

## Neknar Naveen Kumar

Developed by **Neknar Naveen Kumar**.

---

# 🔗 Connect

### LinkedIn

https://www.linkedin.com/in/neknar-naveen-kumar-2271a23b5

---

# 📜 License

This project is created for **academic and demonstration purposes**.
