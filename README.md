# EduManage — School Management & Learning Platform

A complete, interactive frontend prototype of a School Management System designed for primary and secondary schools (with configurable support for Kenyan CBC and other grading systems).

**Repository**: https://github.com/GEDIONKIPCHUMBA/EduManage-School-Management-System

**Live Demo**: Open `index.html` in a modern browser (or serve via any static host / GitHub Pages).

## Features Implemented

### Core Modules
- **Dashboard** – Real-time statistics, interactive Chart.js charts, recent activity feed, filters
- **Student Management** – Full CRUD, detailed profiles with tabs (academics, attendance, fees, personal), search/filter, promote/transfer/archive
- **Teacher Management** – Profiles, subject/class assignments, workload overview
- **Classes & Streams** – Create/manage classes, streams, assign class teachers
- **Subjects** – Register subjects, assign to classes/teachers
- **Examination & Marks** – Exam setup, bulk marks entry, auto-grade calculation, results processing
- **Report Cards** – Generate individual/class reports, printable A4 layout, teacher/principal comments
- **Timetable** – Configuration, conflict-aware generation (basic), class & teacher views, manual edit
- **Attendance** – Daily class register, present/absent/late, analytics, frequent absentees
- **Fees & Payments** – Fee structures, student statements, payment recording, outstanding balances, receipts
- **Assignments & Homework** – Create, assign, submit, mark, status tracking
- **Library** – Books, borrow/return, overdue tracking
- **Announcements** – Targeted publishing (school/class/role)
- **Discipline Records**
- **School Events**
- **Academic Analytics** – Performance by class/subject, trends, support indicators
- **Notifications** – Role-aware alerts with unread indicators
- **Documents**
- **Settings & User Management**

### Portals
- **Admin / Principal / Deputy** – Full access
- **Teacher / Class Teacher** – Assigned classes, marks, attendance, assignments, comments
- **Parent** – Linked children only (performance, attendance, fees, reports, announcements)
- **Student** – Own profile, timetable, results, homework, progress

### Technical Highlights
- Pure HTML5 + CSS3 + Vanilla JavaScript (modular)
- Custom design system (no heavy frameworks)
- Chart.js for interactive analytics
- LocalStorage for all demo data (persistent across sessions)
- Role-based access control (frontend enforced + data filtering)
- Responsive design (desktop / tablet / mobile)
- Dark / Light mode toggle (persisted)
- Smooth transitions, toasts, modals, skeleton states

## Demo Accounts

| Username     | Password     | Role          |
|--------------|--------------|---------------|
| admin        | admin123     | Super Admin   |
| principal    | principal1   | Principal     |
| teacher1     | teacher123   | Teacher       |
| classteacher | class123     | Class Teacher |
| accountant   | accounts1    | Accountant    |
| parent1      | parent123    | Parent        |
| student1     | student123   | Student       |

## How to Run

1. Clone the repository
2. Open `index.html` directly in a browser **or**
3. Serve with any static server:
   ```bash
   npx serve .
   # or
   python -m http.server 8080
   ```
4. Login with any demo account above

## Project Structure

```
EduManage/
├── index.html
├── css/
│   └── styles.css          # Design system + dark mode
├── js/
│   ├── data.js             # Sample data + LocalStorage layer
│   ├── auth.js             # Login + role-based permissions
│   ├── utils.js            # Helpers, toasts, modals, formatters
│   ├── modules.js          # All feature modules (dashboard, students, exams...)
│   └── app.js              # Router, layout, navigation
└── README.md
```

## Future / Production Roadmap
- Backend API + database
- Real authentication (JWT / session)
- File uploads (photos, documents, assignment submissions)
- PDF generation (jsPDF / server-side)
- Payment gateway integration
- SMS / Email notifications
- CBC competency tracking enhancements
- Multi-school / multi-tenant support

---

Built as a comprehensive interactive prototype demonstrating a fully interconnected school management platform.
