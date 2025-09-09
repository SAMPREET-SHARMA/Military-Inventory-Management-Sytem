# Military Inventory Management System

A full-stack **React + Node.js + Express + SQL** project for managing military inventory, supplier requests, and battalion allocations.  
The system provides role-based authentication for **Admin, Manager, Supplier, and Battalion** users.

---

## 🚀 Features

### 🔐 Authentication & Authorization
- Role-based access control (Admin, Manager, Supplier, Battalion)

### 📦 Inventory Management
- **Admin**: Allocate resources to battalions
- **Battalion**: Place requests for resources
- **Supplier**: Fulfill resource requests when stock is insufficient
- **Manager**: Manage suppliers, products, and users

### 📊 Reporting
- Generate daily, weekly, monthly, and yearly reports

---

## 🛠️ Tech Stack

**Frontend:** React (Vite), React Router, Fetch/Axios  
**Backend:** Node.js, Express.js  
**Database:** MySQL / PostgreSQL (via `database.js`)  
**Auth:** JWT (JSON Web Tokens)  

---
## 📂 Project Structure
```
Military-Inventory-Management-System/
├── api/ # Backend (Node + Express)
│ ├── controllers/ # Business logic
│ ├── routes/ # Express routes
│ ├── database.js # Database connection
│ ├── index.js # Backend entry point
│ └── package.json
│
├── client/ # Frontend (React + Vite)
│ ├── src/ # React components
│ ├── index.html # Main HTML file
│ ├── vite.config.js # Vite config
│ └── package.json
│
└── README.md # Project documentation
```
---
## Setup 
Backend (API)

```
cd api
npm install
npm start
```

The backend will run on http://localhost:3000 by default.

Frontend (React)
```
cd client
npm install
npm run dev
```

The frontend will run on http://localhost:5173 by default.

🔑 Environment Variables

Create a .env file inside the /api folder with the following keys:
```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=military_inventory
JWT_SECRET=yourjwtsecret
PORT=3000
```
