# 🎓 EduTrack Pro — School Academic & Examination Management Platform

> A comprehensive digital examination and academic management platform built to modernize how Sri Lankan schools manage student performance, teacher records, and parent communication — replacing traditional paper-based processes with a centralized, role-driven web system.

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![jQuery](https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

---

## 📌 Overview

EduTrack Pro is a SaaS-ready academic management product designed and developed for sale to schools across Sri Lanka. The platform digitizes the entire lifecycle of school term examinations — from entering marks and calculating grade averages to generating class rankings, academic reports, and parent-facing dashboards. It eliminates the manual, paper-heavy workflows currently standard in Sri Lankan schools and replaces them with a fast, reliable, multi-role web application.

The system is architected to serve multiple schools as independent tenants, each managing their own student populations, teacher panels, examination cycles, and academic calendars through a clean, role-based interface.

---

## 🧩 Core Features

### 📊 Examination & Marks Management
- Enter, edit, and publish subject-wise marks for each student per term
- Automatic grade calculation based on configurable grading rubrics (A, B, C, D, F or custom scales)
- Class and batch-wide average calculations updated in real time
- Rank generation — per subject, per class, and across the full batch/year group

### 👩‍🏫 Teacher Management
- Onboard and manage teacher accounts with subject and class assignments
- Role-based access: teachers can only view and edit data within their assigned classes/subjects
- Teacher activity logs for accountability

### 🧑‍🎓 Student Management
- Complete student profiles with enrollment details, class assignment, and academic history
- Track student academic progress across multiple terms and academic years
- Promotion and batch transition management

### 👨‍👩‍👧 Parents Portal
- Dedicated parent-facing portal with secure login
- Real-time access to their child's marks, grades, class rank, and teacher remarks
- Notification system for result publications and school announcements

### 📋 Reports & Analytics
- Auto-generated term report cards (PDF-ready)
- Class performance summaries for school management
- Subject-wise analytics showing pass/fail rates and score distributions
- Batch-level academic health dashboards for principals and administrators

### 🔐 Role-Based Access Control
| Role | Capabilities |
|------|-------------|
| **Super Admin** | Full system control, school configuration |
| **School Admin** | User management, term setup, report generation |
| **Teacher** | Marks entry for assigned classes/subjects |
| **Parent** | View child's results and school communications |

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Backend Framework** | Laravel (PHP) |
| **Frontend** | Blade Templates, jQuery, Bootstrap 5 |
| **Database** | MySQL |
| **Authentication** | Laravel Auth with role-based guards |
| **PDF Generation** | DomPDF / Laravel Excel for reports |
| **Deployment** | Shared/VPS hosting |

---

## 🏗️ Architecture

The system follows a classic **MVC (Model-View-Controller)** architecture using Laravel's Eloquent ORM for database interactions. Key design decisions include:

- **Multi-school tenancy** — Each school operates in an isolated data environment with its own configuration
- **Configurable grading engine** — Grading thresholds, subject weightings, and pass/fail criteria are set per school
- **Hierarchical data model** — School → Batch/Year → Class → Student → Subject → Mark, enabling granular queries at every level
- **Automated ranking engine** — Re-calculates and re-ranks all students in a class/batch upon every mark update

---

## 📸 System Modules

```
EduTrack Pro
├── Authentication & Role Management
├── School Configuration
│   ├── Academic Year & Term Setup
│   ├── Subject & Class Management
│   └── Grading Scale Configuration
├── Student Module
│   ├── Student Enrollment & Profiles
│   └── Batch Promotion
├── Teacher Module
│   ├── Class & Subject Assignment
│   └── Marks Entry Interface
├── Examination Module
│   ├── Mark Entry & Validation
│   ├── Grade Calculation Engine
│   └── Rank Generation Engine
├── Reports Module
│   ├── Term Report Cards (PDF)
│   ├── Class Performance Reports
│   └── Batch Analytics Dashboard
└── Parents Portal
    ├── Secure Login
    ├── Child Results View
    └── Notification Center
```

---

## 💼 Business Context

This platform was developed as a **commercial SaaS product** targeting the Sri Lankan K-12 education sector. The current manual process relies entirely on paper — marks are recorded by hand, rankings are calculated manually, and report cards are typed or written individually. EduTrack Pro replaces all of this with a system that:

- Reduces teacher administrative workload by automating mark aggregation and ranking
- Gives parents instant, transparent access to their child's academic standing
- Provides school management with data-driven insights into academic performance

---

## 🚀 Key Achievements

- Engineered a **configurable grading and ranking engine** capable of processing entire class sets in real time, replacing manual paper-based calculations used across Sri Lankan schools
- Designed a **multi-role access control system** that cleanly separates data access for Super Admins, School Admins, Teachers, and Parents within a single platform
- Developed an **automated report card generation pipeline** producing formatted, print-ready PDF term reports for individual students and class-level summaries
- Architected a **multi-tenant data model** supporting multiple schools on a single platform with isolated configurations, student populations, and academic calendars
- Built a **parent portal** providing secure, real-time visibility into student performance — eliminating the need for physical report collection visits


---

> Built for modernize education administration in Sri Lanka.
