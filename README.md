# Sweet Shop Management System 🍬

The Sweet Shop Management System is a full-stack web application that allows users to browse and purchase sweets, while admin users can manage the sweets inventory. The project demonstrates real-world full-stack development using modern web technologies with secure authentication and role-based access control.

---

## 📌 Project Overview

- Users can register and log in securely
- Users can view available sweets and purchase them
- Admins can add, update, delete, and restock sweets
- JWT-based authentication is used for security
- Frontend and backend are integrated using REST APIs

This project is suitable for academic submission, interviews, and portfolio demonstration.

---

## 🛠️ Tech Stack

### Frontend
- React (Vite)
- Axios
- HTML, CSS

### Backend
- Node.js
- Express.js
- MongoDB (Mongoose)
- JWT Authentication

### Tools
- Git & GitHub
- Nodemon
- Postman / Thunder Client

---

## 📂 Project Structure (Monorepo)

sweet-shop-management-system/
├── backend/
│ ├── config/
│ ├── middleware/
│ ├── models/
│ ├── routes/
│ ├── server.js
│ └── package.json
│
├── frontend/
│ ├── src/
│ ├── public/
│ ├── index.html
│ └── package.json
│
└── README.md

---

## ⚙️ Setup Instructions (Run Locally)

### 🔹 Prerequisites
- Node.js (v16 or above)
- MongoDB (local or MongoDB Atlas)
- Git

---

### 🔹 Backend Setup

```bash
cd backend
npm install
npx nodemon server.js

Backend will run on:
http://localhost:5000

Frontend Setup
Open a new terminal:
cd frontend
npm install
npm run dev

Frontend will run on:
http://localhost:5173

🔐 Authentication Flow
User registers with email and password
Password is hashed and stored in MongoDB
User logs in with credentials
Backend generates a JWT token
Token is stored in browser localStorage
Token is sent in Authorization header
Backend verifies token for protected routes

🔗 API Endpoints
Authentication
POST /api/auth/register
POST /api/auth/login

Sweets
GET /api/sweets
POST /api/sweets (Admin only)
PUT /api/sweets/:id (Admin only)
DELETE /api/sweets/:id (Admin only)

Inventory
POST /api/sweets/:id/purchase
POST /api/sweets/:id/restock (Admin only)

🧪 Test Report
Testing was performed using Postman / Thunder Client.
Test Results
Feature	Status
User Registration	✅ Passed
User Login	✅ Passed
JWT Authentication	✅ Passed
Admin Authorization	✅ Passed
Add Sweet	✅ Passed
Purchase Sweet	✅ Passed
Out-of-Stock Handling	✅ Passed

All major functionalities were tested successfully.

👩‍💻 Author
Vanshika Salaria
