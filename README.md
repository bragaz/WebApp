
# 🎓 High School Management System - Web App

This is a web application developed with React, HTML, CSS, and JavaScript, aimed at facilitating the management of classes, students, teachers, announcements, and attendance in a high school environment.

## 📌 Features

* Register and list students
* Record attendance with date, time, and location
* Publish announcements by class or student
* Dashboard for classes and subjects
* Simple, responsive, and user-friendly interface

---

## 🚀 Technologies Used

* React
* JavaScript (ES6+)
* HTML5
* CSS3
* React Router
* Axios
* JSON Server (for local API simulation)

---

## 🛠️ Installation Guide

Follow the steps below to run the project locally:

### ✅ Prerequisites

* Node.js v18+
* NPM v9+
* Git installed

### 📦 Steps

1. Clone the repository:

```bash
git clone https://github.com/bragaz/sistema-escolar.git
```

2. Navigate into the project folder:

```bash
cd sistema-escolar
```

3. Install dependencies:

```bash
npm install
```

4. Start the development server:

```bash
npm run dev
```

5. Open `http://localhost:5173` in your browser.

---

## 🔌 API Reference

The application uses a REST API simulated with JSON Server. The main available endpoints are:

### 🔹 Base URL

```
http://localhost:3000/api
```

---

### 📄 GET `/students`

Returns all registered students.

**Response:**

```json
[
  {
    "id": 1,
    "name": "João Silva",
    "class": "3ºA"
  }
]
```

---

### ➕ POST `/students`

Registers a new student.

**Body:**

```json
{
  "name": "Maria Oliveira",
  "class": "2ºB"
}
```

---

### 📄 GET `/presences`

Returns all recorded attendance entries.

**Response:**

```json
[
  {
    "id": 1,
    "student": "João Silva",
    "class": "3ºA",
    "summary": "Math Class",
    "date": "2025-06-05",
    "location": "Room 202"
  }
]
```

---

### ➕ POST `/presences`

Creates a new attendance record.

**Body:**

```json
{
  "student": "Maria Oliveira",
  "class": "2ºB",
  "summary": "Biology Class",
  "date": "2025-06-06",
  "location": "Room 101"
}
```

---

### 📄 GET `/announcements`

Returns all announcements.

---

### ➕ POST `/announcements`

Creates a new announcement.

**Body:**

```json
{
  "content": "History exam next Monday",
  "class": "1ºC",
  "date": "2025-06-06",
  "author": "School Board"
}
```

---

## 🤝 Contribution Guide

Contributions are welcome! If you'd like to help improve this system, follow the steps below:

### 📌 Requirements

* Node.js installed
* Basic knowledge of React, JS, HTML, and CSS
* Good communication and clean commit messages

### 🚀 How to Contribute

1. Fork this repository

2. Create a new branch:

```bash
git checkout -b feature/your-feature-name
```

3. Make your changes and commit:

```bash
git commit -m "feat: add new feature"
```

4. Push to your forked repository:

```bash
git push origin feature/your-feature-name
```

5. Open a **Pull Request** with a clear explanation of your changes.

---

### 🧹 Best Practices

* Write clear and objective commits
* Test your code before submitting
* Add comments where necessary
* Follow the project’s code style and structure

---

## 👥 Team Members

* Josivaldo Braga
* Edson Nascimento
* João Guilherme
* Ruan Ribeiro
* Gian Vitor

---

## 📄 License

This project is for educational purposes only and does not currently have a commercial license.

---

## 📬 Contact

For questions or suggestions, open an [Issue](https://github.com/bragaz/sistema-escolar/issues) or email us at `jbragaz@outlook.com`.

---
