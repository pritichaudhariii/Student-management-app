# 🎓 Student Management App

A full-stack web application for managing student and course records, built with a Node.js/Express backend and an HTML/CSS/JavaScript frontend.

## ✨ Features

- 👩‍🎓 **Student Management** — Add, edit, delete, and search students by name, email, or course
- 📚 **Course Management** — Create and manage courses with descriptions, duration, and active/inactive status
- 📊 **Dashboard Analytics** — View real-time stats including total students, active enrollments, course counts, and graduation success rate
- 🔍 **Live Search** — Debounced search across student records
- 💓 **Health Monitoring** — Built-in health check endpoints (`/health`, `/health/detailed`) reporting server uptime, memory usage, and database connection status
- 📝 **Logging** — Winston-based structured logging (errors, requests, and application events) alongside Morgan HTTP request logging

## 🛠️ Tech Stack

- **Backend:** Node.js, Express, Mongoose (MongoDB ODM)
- **Database:** MongoDB
- **Frontend:** HTML5, CSS3, vanilla JavaScript (Fetch API)
- **Logging:** Winston, Morgan

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET/POST | `/api/students` | List and create students |
| PUT/DELETE | `/api/students/:id` | Update and delete a student |
| GET | `/api/students/search?q=` | Search students |
| GET/POST | `/api/courses` | List and create courses |
| PUT/DELETE | `/api/courses/:id` | Update and delete a course |
| GET | `/api/dashboard/stats` | Aggregate dashboard statistics |
| GET | `/health`, `/health/detailed` | Server/database health checks |
