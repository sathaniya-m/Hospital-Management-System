# 🏥 Hospital Management Database System (HMS)

A comprehensive, full-stack web application designed to digitalize hospital operations. This system streamlines the appointment booking process for patients, provides doctors with an organized schedule, and offers an administrative dashboard to manage hospital database records in real-time.

## 📑 Table of Contents
- [About the Project](#-about-the-project)
- [Key Features](#-key-features)
- [Technology Stack](#-technology-stack)
- [Folder Structure](#-folder-structure)
- [Prerequisites](#-prerequisites)
- [Installation & Setup](#-installation--setup)
- [Usage Guide](#-usage-guide)
- [Screenshots](#-screenshots)
- [Future Enhancements](#-future-enhancements)

---

## 📖 About the Project
The Hospital Management Database System bridges the gap between patients and healthcare providers. It provides a secure platform where patients can view available doctors, book specific time slots, and manage their health concerns. Administrators and authorized medical staff can access backend database logs to perform CRUD (Create, Read, Update, Delete) operations on patient appointments.

---

## ✨ Key Features

**For Patients:**
* 🔐 **Secure Authentication:** User registration and login functionality.
* 📅 **Slot Booking:** Interactive form to select doctors, departments, dates, and times.
* 👨‍⚕️ **Doctor Directory:** View available specialists before booking.

**For Administration & Doctors:**
* 📊 **Centralized Dashboard:** View all active patient bookings in a clean tabular format.
* ✏️ **Record Management (CRUD):** Edit existing patient details or update diagnoses dynamically.
* 🗑️ **Data Deletion:** Securely delete canceled or completed appointments from the database.
* 🛡️ **Role-Based Access Control:** Restricted views ensuring only authorized users can access sensitive database tables.

---

## 🛠 Technology Stack

**Frontend (Client-Side):**
* **HTML5 & CSS3:** For structuring and styling the web pages.
* **Bootstrap 4/5:** For a responsive, mobile-friendly user interface.
* **Jinja2:** Server-side templating to dynamically render database queries into HTML.

**Backend (Server-Side):**
* **Python 3.x:** Core programming logic.
* **Flask:** Lightweight WSGI web application framework.
* **Flask-Login:** User session management.

**Database Management:**
* **MySQL:** Relational database for storing users, doctors, and booking entities.
* **SQLAlchemy / Flask-MySQLdb:** For database connection and executing raw/ORM SQL queries.

---

## 📂 Folder Structure

```text
Hospital-System/
│
├── static/                   # Static assets (CSS, JavaScript, Images)
│   ├── css/
│   │   └── virtualregister.css
│   └── images/               # UI and Doctor placeholder images
│       ├── doc.jpg
│       ├── h14.jpg
│       └── h20.jpg
│
├── templates/                # Jinja2 HTML Templates
│   ├── base.html             # Base layout & Navigation Bar
│   ├── index.html            # Landing Page
│   ├── login.html            # User/Doctor Login
│   ├── signup.html           # Registration Page
│   ├── patient.html          # Appointment Booking Form
│   ├── booking.html          # Admin/Doctor Database Dashboard
│   ├── edit.html             # Update Booking details
│   └── trigers.html          # Database trigger logs
│
├── main.py                   # Main Flask Application & Routing
├── hms.sql                   # MySQL Database Backup/Schema File
├── requirements.txt          # Python project dependencies
└── README.md                 # Project documentation
