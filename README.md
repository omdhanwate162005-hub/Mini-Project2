📘 Employee Management System (EMS)
🔷 Project Description

The Employee Management System (EMS) is a full-stack web application designed to manage employee records efficiently. It allows administrators to perform CRUD operations (Create, Read, Update, Delete) on employee data with a secure authentication system.

🚀 Tech Stack
🔹 Frontend
HTML5
CSS3
JavaScript
React.js
Bootstrap / Tailwind CSS
🔹 Backend
Node.js
Express.js
🔹 Database
MySQL
🔹 Other Tools
JWT (Authentication)
bcrypt (Password Hashing)
Axios (API Calls)
✨ Features
🔐 User Authentication (Login/Logout)
👨‍💼 Add Employee
📋 View Employees
✏️ Update Employee Details
❌ Delete Employee
🔍 Search & Filter Employees
📊 Dashboard Statistics
📱 Responsive Design
📂 Project Structure
EMS-Project/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   ├── config/
│   └── package.json
│
├── database/
│   └── ems.sql
│
└── README.md
⚙️ Installation & Setup
🔹 Step 1: Clone Repository
git clone https://github.com/your-username/ems-project.git
cd ems-project
🔹 Step 2: Setup Backend
cd backend
npm install

Create .env file in backend:

PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=ems
JWT_SECRET=your_secret_key

Run backend:

npm start
🔹 Step 3: Setup Frontend
cd frontend
npm install
npm start
🔹 Step 4: Setup Database

Open MySQL and run:

CREATE DATABASE ems;
USE ems;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50),
    password VARCHAR(255)
);

CREATE TABLE employees (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    department VARCHAR(100),
    salary DOUBLE,
    phone VARCHAR(15)
);
🔑 Default Login
Username: admin
Password: admin123

(Make sure to insert this user manually with hashed password or update code accordingly)

📡 API Endpoints
Method	Endpoint	Description
POST	/api/login	User login
GET	/api/employees	Get all employees
POST	/api/employees	Add employee
PUT	/api/employees/:id	Update employee
DELETE	/api/employees/:id	Delete employee
🛠️ Future Enhancements
Role-based access control
Export data (PDF/Excel)
Profile images upload
Email notifications
Advanced analytics dashboard
🧠 Learning Outcomes
Understanding of full-stack development
Working with REST APIs
Database integration with MySQL
Authentication using JWT
CRUD operations
