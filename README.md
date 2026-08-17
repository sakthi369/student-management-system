🎓 Student Management System

A full-stack Student Management System developed as a web development project to efficiently manage student records, academic information, departments, and student data through a centralized web application.

The system provides a clean dashboard, student CRUD operations, search and department filtering, and a responsive user interface.

---

📌 Project Overview

The Student Management System is designed to simplify the process of maintaining student records.

Administrators or staff can:

- View all student records
- Add new students
- Edit existing student information
- Delete student records
- Search students
- Filter students by department
- View student statistics through a dashboard
- Access the application through a responsive web interface

The project follows a frontend + backend + database architecture using REST APIs.

---

✨ Features

🏠 Home Page

- Professional landing page
- Project overview
- Quick navigation to Dashboard and Students
- Technology overview
- Responsive design

📊 Dashboard

- Total student count
- Department-wise student statistics
- CSE student count
- ECE student count
- IT student count
- Department overview with progress indicators
- Recent student records
- Quick action buttons
- System information

👨‍🎓 Student Management

Complete CRUD functionality:

- Create — Add a new student
- Read — View student records
- Update — Edit student information
- Delete — Remove student records

🔎 Search & Filtering

Students can be searched using:

- Name
- Department
- Email
- Phone number

Students can also be filtered according to department.

📱 Responsive UI

The application is designed to work across:

- Desktop
- Laptop
- Tablet
- Mobile devices

---

🛠️ Technologies Used

Frontend

- React.js
- Vite
- JavaScript
- HTML5
- CSS3
- Axios
- React Router

Backend

- Node.js
- Express.js
- REST API
- CORS
- dotenv

Database

- MySQL

Development Tools

- Visual Studio Code
- Git
- GitHub
- npm

---

🏗️ Project Architecture

Student Management System
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   ├── api.js
│   │   └── index.css
│   │
│   ├── package.json
│   └── vite.config.js
│
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── config/
│   ├── server.js
│   ├── package.json
│   └── .env
│
├── .gitignore
└── README.md

«The exact internal folder structure may vary depending on the current implementation.»

---

🔄 Application Flow

User
 │
 ▼
React Frontend
 │
 │ Axios HTTP Requests
 ▼
Node.js + Express Backend
 │
 │ REST API
 ▼
MySQL Database
 │
 ▼
Student Records

---

🗄️ Student Database Structure

The student records contain information such as:

Field| Description
"id"| Unique student ID
"name"| Student name
"age"| Student age
"department"| Academic department
"email"| Student email
"phone"| Contact number
"year"| Academic year
"created_at"| Record creation date

---

🔌 API Endpoints

Get all students

GET /api/students

Add a student

POST /api/students

Update a student

PUT /api/students/:id

Delete a student

DELETE /api/students/:id

---

📦 Installation

1. Clone the repository

git clone https://github.com/sakthi369/student-management-system.git

Move into the project:

cd student-management-system

---

⚙️ Backend Setup

Go to the backend directory:

cd backend

Install dependencies:

npm install

Create a ".env" file:

PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=student_management

«Do not upload the ".env" file to GitHub.»

Start the backend:

npm start

The backend will run on:

http://localhost:5000

---

💻 Frontend Setup

Open another terminal.

Go to the frontend:

cd frontend

Install dependencies:

npm install

Start the Vite development server:

npm run dev

The frontend will normally be available at:

http://localhost:5173

---

🗃️ Database Setup

Create the database in MySQL:

CREATE DATABASE student_management;

Select the database:

USE student_management;

Create the students table:

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    age INT NOT NULL,
    department VARCHAR(100) NOT NULL,
    email VARCHAR(150) NOT NULL UNIQUE,
    phone VARCHAR(20) NOT NULL,
    year INT NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

Verify the table:

DESCRIBE students;

---

▶️ Running the Complete Application

You need two terminals.

Terminal 1 — Backend

cd backend
npm install
npm start

Terminal 2 — Frontend

cd frontend
npm install
npm run dev

Then open:

http://localhost:5173

---

🧪 Testing

The following functionality can be tested:

Student Creation

1. Open the Add Student page.
2. Enter student details.
3. Click Add Student.
4. Verify that the student appears in the student list.

Student Update

1. Open Students.
2. Click Edit.
3. Modify student information.
4. Save the changes.
5. Verify the updated record.

Student Deletion

1. Open Students.
2. Click Delete.
3. Confirm deletion.
4. Verify that the student is removed.

Search

Enter a student name, department, email, or phone number in the search field.

Department Filter

Select a department from the department filter and verify the displayed records.

---

🔐 Environment Variables

The backend uses environment variables for database configuration.

Example:

PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=student_management

Sensitive files such as ".env" should never be committed to GitHub.

---

🚀 Deployment

The project can be deployed using free hosting platforms.

Frontend

The React + Vite frontend can be deployed using:

- Netlify
- Vercel

Backend

The Node.js + Express backend can be deployed using:

- Render
- Railway
- Other Node.js hosting platforms

Database

The MySQL database can be hosted using a cloud MySQL provider.

The frontend and backend should use environment variables for production API URLs and database credentials.

---

📈 Future Improvements

Possible future enhancements include:

- User authentication
- Admin and faculty roles
- JWT authentication
- Password encryption
- Student profile pages
- Attendance management
- Marks management
- Course management
- Export student records to PDF/Excel
- Pagination
- Advanced analytics
- Dark mode
- Cloud database integration
- Production deployment

---

🎯 Learning Outcomes

This project helped demonstrate practical knowledge of:

- React component development
- React Router
- REST API development
- Node.js and Express
- MySQL database integration
- CRUD operations
- Axios API communication
- Search and filtering
- Responsive web design
- Git and GitHub
- Full-stack web application development

---

👨‍💻 Developer

Sakthi

GitHub:

https://github.com/sakthi369

Project Repository:

https://github.com/sakthi369/student-management-system

---

📄 License

This project is developed for educational and internship purposes.
