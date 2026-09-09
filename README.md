# Learnova – Learning Management System

> Learn. Grow. Achieve.

Learnova is a modern full-stack Learning Management System designed to provide a complete digital learning experience for students, teachers, and administrators.

The application supports role-based authentication, course management, lessons, assignments, quizzes, student progress tracking, and administrative management.

---

## 🚀 Features

### 🔐 Secure Authentication

- JWT-based authentication
- BCrypt password encryption
- Role-Based Access Control (RBAC)
- Separate dashboards for Admin, Teacher, and Student

### 👨‍💼 Admin Dashboard

- Manage students and teachers
- View platform statistics
- Monitor course categories
- Activate or deactivate users
- Assign or reassign teachers to courses
- View enrollment information

### 👨‍🏫 Teacher Dashboard

- Create and manage courses
- Add course descriptions and thumbnails
- Upload learning materials
- Create lessons
- Create assignments
- Create quizzes and MCQ questions
- Evaluate student submissions

### 👨‍🎓 Student Dashboard

- Browse available courses
- Enroll in courses
- Access course lessons
- Track learning progress
- Submit assignments
- Attempt quizzes
- Download learning materials
- View certificates

### 📚 Course Management

Learnova supports multiple courses across different technologies and subjects.

Sample courses include:

- Web Development
- Java Programming
- MySQL Database Management

---

## 🛠️ Tech Stack

### Backend

| Technology | Usage |
|---|---|
| Java 21 | Programming Language |
| Spring Boot 3.3.1 | Backend Framework |
| Spring Security | Authentication & Authorization |
| Spring Data JPA | Database Operations |
| Hibernate | ORM |
| MySQL | Database |
| JWT | Secure Authentication |
| Lombok | Boilerplate Reduction |
| Swagger / OpenAPI | API Documentation |
| Maven | Dependency Management |

### Frontend

| Technology | Usage |
|---|---|
| React.js | Frontend Framework |
| Vite | Build Tool |
| React Router DOM | Routing |
| Axios | API Communication |
| Tailwind CSS | Styling |
| Lucide React | Icons |
| Recharts | Dashboard Charts |

---

## 👥 User Roles

Learnova provides three different user roles.

### 👑 Admin

Administrators can:

- Manage users
- Manage teachers and students
- Monitor courses
- Assign teachers
- View enrollment data
- Activate or deactivate users

### 👨‍🏫 Teacher

Teachers can:

- Create courses
- Add lessons
- Upload course materials
- Create assignments
- Create quizzes
- Evaluate student submissions

### 👨‍🎓 Student

Students can:

- Browse courses
- Enroll in courses
- Access learning materials
- Complete lessons
- Submit assignments
- Attempt quizzes
- Track progress
- View certificates

---

## 🔑 Default Test Credentials

When the backend starts for the first time, the DatabaseSeeder automatically creates default users.

| Role | Username | Email | Password |
|---|---|---|---|
| Admin | admin | admin@lms.com | admin123 |
| Teacher | teacher | teacher@lms.com | teacher123 |
| Student | student | student@lms.com | student123 |

> These credentials are intended only for development and testing.

---

## 📂 Project Structure

```text
learnova-lms/
│
├── backend/
│   ├── pom.xml
│   └── src/
│       └── main/
│           ├── java/com/lms/digital/
│           │   ├── config/
│           │   ├── controller/
│           │   ├── dto/
│           │   ├── entity/
│           │   ├── exception/
│           │   ├── mapper/
│           │   ├── repository/
│           │   └── security/
│           │
│           └── resources/
│               ├── application.properties
│               ├── schema.sql
│               └── data.sql
│
├── frontend/
│   ├── package.json
│   ├── vite.config.js
│   ├── tailwind.config.js
│   ├── index.html
│   │
│   └── src/
│       ├── components/
│       ├── context/
│       ├── hooks/
│       ├── pages/
│       ├── routes/
│       ├── services/
│       ├── App.jsx
│       └── main.jsx
│
└── README.md