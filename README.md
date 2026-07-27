#  Student Management App

A full-stack web application for managing student and course records, built with a Node.js/Express backend and a vanilla JavaScript frontend.

# Features
- Student Management — Add, edit, delete, and search students by name, email, or course
- Course Management — Create and manage courses with descriptions, duration, and active/inactive status
- Dashboard Analytics — View real-time stats including total students, active enrollments, course counts, and graduation success rate
- Live Search — Debounced search across student records
- Health Monitoring — Built-in health check endpoints (/health, /health/detailed) reporting server uptime, memory usage, and database connection status
- Logging — Winston-based structured logging (errors, requests, and application events) alongside Morgan HTTP request logging

# Tech Stack
- Backend: Node.js, Express, Mongoose (MongoDB ODM)
- Database: MongoDB
- Frontend: HTML, CSS, vanilla JavaScript (Fetch API)
- Logging: Winston, Morgan

# API Endpoints
- GET/POST /api/students — list and create students
- PUT/DELETE /api/students/:id — update and delete a student
- GET /api/students/search?q= — search students
- GET/POST /api/courses — list and create courses
- PUT/DELETE /api/courses/:id — update and delete a course
- GET /api/dashboard/stats — aggregate dashboard statistics
- GET /health and /health/detailed — server/database health checks
