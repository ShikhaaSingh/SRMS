# SRMS — AI-Powered Student Result Management System

A full-stack web application for managing student academic records, results, grades, and performance analytics.

Built with **Java, Spring Boot, MongoDB, HTML5, CSS3, and JavaScript**, SRMS provides RESTful APIs and a simple web interface to reduce manual result-management work and make student performance analysis easier.

## 🚀 Features

* 👨‍🎓 Manage student academic records
* 📊 Manage grades and examination results
* 🔄 CRUD operations through RESTful APIs
* 📈 Student performance analytics
* 🗄️ MongoDB-based data storage
* ⚡ Fast backend API responses
* 🌐 Responsive web interface
* 🤖 AI-assisted development using ChatGPT
* 🏗️ Clean MVC-based application structure

## 🛠️ Tech Stack

**Backend**

* Java
* Spring Boot
* REST APIs
* Maven

**Database**

* MongoDB

**Frontend**

* HTML5
* CSS3
* JavaScript

**Development Tools**

* Git & GitHub
* ChatGPT for AI-assisted development

## 📌 Project Highlights

### Student Result Management

Built the application to manage academic records and examination results for **500+ student records**, reducing repetitive manual data-entry work.

### RESTful Backend

Developed **5+ RESTful APIs** supporting CRUD operations for student and result management.

### Performance Analytics

Implemented performance analytics features to help analyze student results and support academic decision-making.

### Database Management

Used **MongoDB** for storing and retrieving student, subject, and result-related information.

### Backend Performance

Designed backend APIs with typical response times of **under 200ms** during development and testing.

### AI-Assisted Development

Used **ChatGPT** as a development assistant for debugging, implementation guidance, code refinement, and documentation, helping reduce development time while maintaining a clean code structure.


## 🏗️ Application Architecture

The application follows a layered MVC-style structure:

```text
                    ┌─────────────────────┐
                    │     Web Browser     │
                    │ HTML/CSS/JavaScript │
                    └──────────┬──────────┘
                               │
                               │ HTTP Requests
                               ▼
                    ┌─────────────────────┐
                    │    REST Controller  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Service Layer    │
                    │ Business Logic      │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Repository Layer  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │      MongoDB        │
                    │    Database         │
                    └─────────────────────┘
```

### Request Flow

```text
User
 ↓
Frontend
 ↓
REST API
 ↓
Controller
 ↓
Service
 ↓
Repository
 ↓
MongoDB
```

## 📁 Project Structure

```text
SRMS/
│
├── src/
│   └── main/
│       ├── java/
│       │   └── ...
│       │
│       └── resources/
│           └── application.properties
│
├── frontend/
│   ├── index.html
│   ├── css/
│   └── js/
│
├── pom.xml
├── README.md
└── .gitignore
```

> The exact package and folder names may vary depending on the current project structure.

### Main Backend Components

| Component         | Responsibility                                  |
| ----------------- | ----------------------------------------------- |
| **Controller**    | Handles HTTP requests and API endpoints         |
| **Service**       | Contains application/business logic             |
| **Repository**    | Handles database operations                     |
| **Model/Entity**  | Represents student and result data              |
| **Configuration** | Contains application and database configuration |


## 🔌 REST API

The backend exposes RESTful APIs for managing student and result information.

### Student APIs

| Method   | Endpoint             | Description            |
| -------- | -------------------- | ---------------------- |
| `GET`    | `/api/students`      | Get all students       |
| `GET`    | `/api/students/{id}` | Get student by ID      |
| `POST`   | `/api/students`      | Create a student       |
| `PUT`    | `/api/students/{id}` | Update student details |
| `DELETE` | `/api/students/{id}` | Delete a student       |

### Example Request

```http
POST /api/students
Content-Type: application/json
```

```json
{
  "name": "Rahul Sharma",
  "rollNumber": "SRMS101",
  "course": "Computer Science"
}
```

### Example Response

```json
{
  "id": "64abc123",
  "name": "Rahul Sharma",
  "rollNumber": "SRMS101",
  "course": "Computer Science"
}
```

> Update the endpoint names and request/response fields above to match the actual implementation in the project.

