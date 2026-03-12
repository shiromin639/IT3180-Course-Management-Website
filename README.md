# IT3180 - Course Management Platform 🎓

A comprehensive full-stack educational web application designed to facilitate online learning and course administration. This platform supports multiple user roles (Admin, Instructor, Student) with secure authentication, course content management, and interactive assignment submissions.

## ✨ Key Features

* **Role-Based Access Control (RBAC):** Distinct dashboards and permissions for Admins, Instructors, and Students.
* **Secure Authentication:** Implementation of Spring Security with JSON Web Tokens (JWT) for stateless authentication and secure API endpoints.
* **Course Content Management:** Instructors can construct courses using a hierarchical structure of Chapters, Lessons, and Exercises.
* **Interactive Learning:** * Students can enroll in courses, view video lessons, and track progress.
  * Built-in discussion and comment sections for each lesson.
* **Assignment System:** Seamless submission of exercises and assignments by students.
* **Responsive UI:** Modern, responsive frontend built with React and custom CSS modules.

## 🛠️ Tech Stack

### Frontend
* **Framework:** React.js (Bootstrapped with Vite for fast HMR)
* **State Management:** React Context API (`AuthProvider`, `ThemeProvider`)
* **Routing:** React Router v6 (`AppRoutes`, Route Guards)
* **Styling:** CSS Modules for scoped styling
* **HTTP Client:** Axios (with custom interceptors for JWT injection)

### Backend
* **Core:** Java 17 / Spring Boot 3
* **Security:** Spring Security & JWT (`AuthTokenFilter`, `AuthEntryPointJwt`)
* **Data Access:** Spring Data JPA / Hibernate
* **Database:** MySQL
* **Testing:** JUnit 5, Mockito, and Integration Testing

---

## 📂 Project Structure

```text
IT3180-Course-Management-Website/
├── backend/                  # Spring Boot REST API
│   ├── src/main/java/...     # Controllers, Services, Models, Repositories, Security
│   ├── src/main/resources/   # application.properties
│   └── src/test/             # Unit and Integration Tests
├── frontend/                 # React UI
│   ├── src/components/       # Reusable UI components (Admin, Course, Dashboard, Layout)
│   ├── src/context/          # Global state (Auth, Theme)
│   ├── src/pages/            # View components (Login, Dashboard, CourseDetail)
│   └── src/api/              # Axios configuration and API calls
└── docs/                     # Project documentation, test reports, and style guides
