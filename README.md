<div align="center">

# 🎓 Academic Management System (ERP)

### Enterprise-grade Academic ERP serving 4,000+ active users in a real-world educational institution

![React](https://img.shields.io/badge/React.js-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)

</div>

---

## 📌 Overview

A comprehensive, enterprise-grade **Academic Management System (ERP)** built for real-world educational institutions. The platform manages the **complete academic lifecycle** — from student enrollment and attendance to financial operations and certificate generation — all in one fully integrated system.

> 🏫 Currently serving **4,000+ active users** across multiple departments in a live production environment.

---

## ✨ Key Features

### 🔐 Role-Based Access Control (RBAC)
Dedicated dashboards for **7 user roles**, each with fully isolated permissions:

| Role | Access |
|------|--------|
| 👑 Owner | Full system control & reports |
| 🛡️ Super Admin | System configuration & management |
| 👤 Admin | Branch operations & oversight |
| 👨‍🏫 Teacher | Classes, attendance & grading |
| 🎓 Student | Personal dashboard & records |
| 📋 Student Affairs | Enrollment & student records |
| 💰 Accounting | Financial operations & invoices |

---

### 📚 Academic Modules
- Student enrollment, courses & diplomas management
- Class scheduling & timetable generation
- Grading system & certificate generation
- Student records & academic history

---

### 🖐️ Dual Attendance Verification System
One of the system's most innovative features:

- 🪪 **ID Card Scanning** — Students register attendance at the academy entrance using their physical ID cards
- 📲 **Dynamic QR Code** — Instructors verify classroom attendance by scanning a QR Code that **automatically refreshes every 10 seconds**, eliminating fraudulent attendance

---

### 💰 Financial Module
- Student payment tracking & invoicing
- Financial documents & purchasing workflows
- Complete financial reporting & analytics

---

### 📊 Interactive Dashboards & Analytics
- Real-time charts powered by **Chart.js**, **Recharts**
- Advanced reporting across all departments
- Data export to **Excel & CSV** formats

---

### 📅 Smart Interactive Calendar
One of the platform's most powerful collaborative features:

- 🖱️ **Drag & Drop scheduling** — Admins can create, move, and reschedule events and lectures directly on the calendar
- 👁️ **Role-aware views** — Every user sees the same calendar but with **personalized content** based on their role:
  - 👑 Owner / Admin → sees all events across all branches
  - 👨‍🏫 Teacher → sees only their assigned lectures & sessions
  - 🎓 Student → sees only their enrolled courses & schedules
- 🔄 **Real-time updates** — Changes reflect instantly for all users
- 📆 Supports events, lectures, exams, and custom academy activities

---

### 🌐 Additional Features
- **Multilingual support** (i18n) — Arabic & English
- **Excel / CSV import & export** for bulk data management
- **QR Code generation** for attendance and documents
- **Secure authentication** with JWT & bcrypt
- Scalable RESTful API architecture

---

## 🛠️ Technologies Used

### Frontend
![React](https://img.shields.io/badge/React.js-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=axios&logoColor=white)
![React Router](https://img.shields.io/badge/React_Router-CA4245?style=flat-square&logo=react-router&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-22B5BF?style=flat-square&logo=react&logoColor=white)
![i18next](https://img.shields.io/badge/i18next-26A69A?style=flat-square&logo=i18next&logoColor=white)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=flat-square&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=flat-square&logo=mysql&logoColor=white)

### Authentication & Security
![JWT](https://img.shields.io/badge/JWT-black?style=flat-square&logo=JSON%20web%20tokens&logoColor=white)
![bcrypt](https://img.shields.io/badge/bcrypt-338?style=flat-square&logo=npm&logoColor=white)

### File Management
![Multer](https://img.shields.io/badge/Multer-FF6C37?style=flat-square&logo=npm&logoColor=white)
![ExcelJS](https://img.shields.io/badge/ExcelJS-217346?style=flat-square&logo=microsoft-excel&logoColor=white)
![PapaParse](https://img.shields.io/badge/PapaParse-FFD700?style=flat-square&logo=npm&logoColor=black)

### Utilities
![QRCode](https://img.shields.io/badge/QRCode-000000?style=flat-square&logo=qrcode&logoColor=white)
![dotenv](https://img.shields.io/badge/dotenv-ECD53F?style=flat-square&logo=dotenv&logoColor=black)
![CORS](https://img.shields.io/badge/CORS-FF6C37?style=flat-square&logo=npm&logoColor=white)

---

## 🏗️ System Architecture

```
ATS/
├── client/                  # React.js Frontend
│   ├── src/
│   │   ├── pages/           # Role-based page views
│   │   ├── components/      # Reusable UI components
│   │   ├── context/         # Global state management
│   │   ├── hooks/           # Custom React hooks
│   │   ├── i18n/            # Multilingual config
│   │   └── utils/           # Helper functions
├── server/                  # Node.js Backend
│   ├── routes/              # API route definitions
│   ├── controllers/         # Business logic
│   ├── middleware/          # Auth & validation
│   ├── config/              # DB & environment config
│   └── utils/               # QR, Excel, helpers
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js v18+
- MySQL 8+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/islamsaeed597/ats-academic-erp.git
cd ats-academic-erp

# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install
```

### Environment Variables

Create a `.env` file in the `/server` directory:

```env
DB_HOST=your_database_host
DB_USER=your_database_user
DB_PASSWORD=your_database_password
DB_NAME=your_database_name
JWT_SECRET=your_jwt_secret
PORT=5000
```

### Run the Application

```bash
# Run backend & frontend concurrently
npm run dev

# Or separately:
# Backend
cd server && npm start

# Frontend
cd client && npm start
```

---

## 📸 Screenshots

> 📌 *Screenshots and demo coming soon*

---

## 👨‍💻 Author

**Eslam Saeed** — Full Stack Developer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/eslam-saeed-b70955317)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=flat-square&logo=github&logoColor=white)](https://github.com/islamsaeed597)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:islamsaeed597@gmail.com)

---

<div align="center">
⭐ If you found this project interesting, please consider giving it a star!
</div>
