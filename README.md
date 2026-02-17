# 🎓 Scholars — K-12 School Management System

A modern, fully-featured school management system built as a single-file HTML application. Designed for K-12 / Primary & Secondary schools with a clean light theme and Windows-friendly interface.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features & Modules](#features--modules)
- [Getting Started](#getting-started)
- [Module Guide](#module-guide)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Customization](#customization)
- [Tech Stack](#tech-stack)
- [File Structure](#file-structure)
- [Screenshots](#screenshots)
- [FAQ](#faq)

---

## Overview

**Scholars** is a zero-dependency, browser-based school management system delivered as a single `.html` file. No installation, no server, no database required — just open the file in any modern browser and you're ready to go.

| Property | Detail |
|---|---|
| **Type** | Single-file HTML App |
| **Target** | K-12 / Primary & Secondary Schools |
| **Theme** | Light / Modern White |
| **Dependencies** | None (Google Fonts via CDN) |
| **Browser Support** | Chrome, Edge, Firefox, Safari (latest) |

---

## Features & Modules

### 1. 🏠 Dashboard
The central overview screen showing school-wide statistics at a glance.

- **4 KPI Cards** — Total students, teaching staff, today's attendance %, and pending fees
- **Quick Action Buttons** — One-click access to common tasks (add student, mark attendance, etc.)
- **Recent Enrollments Table** — Latest students with GPA and status
- **Today's Schedule** — Current day's class timetable for Grade 10-A
- **Weekly Attendance Bar Chart** — Visual attendance trend for the current week (Mon–Fri)
- **Fee Collection Progress** — Progress bars per fee category (Tuition, Exam, Sports, Library)

---

### 2. 🎒 Students & Enrollment
Full student roster with enrollment management.

- View all 1,248+ enrolled students in a sortable table
- **Student details**: ID, class & section, parent phone, GPA, and status (Active/Inactive)
- **Color-coded GPA** — Green (≥3.7), Blue (≥3.0), Amber (below 3.0)
- **Class filter** — Filter by Grade 9, 10, 11, or 12
- **Global search** — Search by name or student ID from the top bar
- **Add new student** via modal form (name, DOB, gender, grade, section, contact, previous school)

---

### 3. 👩‍🏫 Teachers & Staff
Staff directory for all teaching and administrative personnel.

- View all 86 staff members with subject, assigned classes, and experience
- Staff status badges: **Active**, **On Leave**
- **Add new staff member** via modal (name, subject, email, phone, experience, qualification)
- Quick links to view profiles or edit records

---

### 4. ✅ Attendance Tracking
Daily attendance management with a weekly view.

- Displays the current week (Mon–Fri) for the selected class
- **Click-to-toggle** attendance buttons — click ✅ to mark absent, ❌ to restore present
- **Auto-calculated weekly %** per student with color coding (Green ≥80%, Red <80%)
- Class selector to switch between sections (Grade 10-A, 10-B, 11-A)
- **Save Attendance** button to confirm records

---

### 5. 📊 Grades & Results
Academic performance tracking and reporting.

- **Subject Performance** — Average score progress bars for all 6 subjects
- **Top Performers Leaderboard** — Top 6 students with gold/silver/bronze medals
- **Full Results Table** — All students with per-subject scores, total out of 400, and letter grade
- Letter grade scale: **A+** (90%+), **A** (80%+), **B+** (70%+), **B** (60%+), **C** (50%+), **D** (below 50%)
- Semester selector (Spring 2026 / Fall 2025)
- **Export PDF** button (ready for backend integration)

---

### 6. 🗓️ Class Timetable
Weekly class schedule in a color-coded grid view.

- 7 time slots × 5 days (Monday–Friday)
- Each cell shows **subject name + teacher name**
- Color coding by subject:
  - 🔵 **Mathematics** — Blue
  - 🟢 **Science** — Teal
  - 🟡 **English** — Amber
  - 🔴 **History** — Rose
  - 🟣 **P.E.** — Violet
  - 🩷 **Art** — Pink
  - Break periods shown in grey italic
- Class selector (Grade 10-A, 11-B, 12-A)
- **Edit Schedule** button (ready for backend integration)

---

### 7. 💳 Fee Management
Track, manage, and collect student fees.

- **3 summary KPI cards** — Amount collected, amount pending, collection rate %
- Outstanding fee records with student name, fee type, due date, and status
- Status badges: **Pending**, **Overdue**, **Paid**
- **Mark Paid** button to update individual fee statuses in real time
- **Add Fee Record** modal — student name, fee type, amount, due date, status
- Tracks: Tuition Fee, Exam Fee, Sports Fee, Library Fee

---

### 8. 📢 Notices & Announcements
Internal communication board for the school.

- Chronological notice board with category icons and color-coded borders
- Notice categories: 📢 General, 🎉 Event, ⚠️ Important, 🏖️ Holiday, 📝 Exam
- **Inline post form** — Title, category, audience, and message body
- Audience targeting: All Students & Parents, specific grades, or Staff Only
- Newly posted notices appear instantly at the top of the board

---

## Getting Started

### Option 1 — Open Directly (Recommended)
1. Download `scholars-k12-school-management.html`
2. Double-click the file — it opens in your default browser
3. For best experience, use **Google Chrome** or **Microsoft Edge**

### Option 2 — Windows Shortcut
1. Right-click the `.html` file → **Send to → Desktop (create shortcut)**
2. Double-click the desktop shortcut to launch the app anytime

### Option 3 — Full-Screen Mode
1. Open the file in your browser
2. Click the **⛶** button in the top-right corner of the app to enter full-screen
3. Press **Esc** to exit full-screen

> **Note:** All data is stored in-memory during the session. Refreshing the page will reset to the default sample data. For persistent storage, integrate a backend or localStorage layer.

---

## Module Guide

### Adding a Student
1. Click **"➕ Add Student"** from the Dashboard or the Students page
2. Fill in: First Name, Last Name, Date of Birth, Gender, Grade, Section, Parent Phone, Email, Previous School
3. Click **"Enroll Student"**
4. The student is added instantly to the top of the Students table

### Posting a Notice
1. Navigate to the **Notices** page
2. Fill in the Title, select a Category and Audience, write the Message
3. Click **"📢 Publish Notice"**
4. The notice appears at the top of the board immediately

### Marking Attendance
1. Go to the **Attendance** page
2. Select the class from the dropdown
3. Click any ✅ to toggle it to ❌ (absent) or vice versa
4. Click **"💾 Save Attendance"** to confirm

### Marking a Fee as Paid
1. Go to **Fee Management**
2. Find the student's outstanding record
3. Click **"✓ Mark Paid"** — the status updates to **Paid** instantly

---

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Esc` | Close any open modal |
| `Ctrl + F` | Focus browser search (for in-page text search) |

---

## Customization

### Changing School Name / Logo
Open the `.html` file in a text editor (Notepad, VS Code, etc.) and find:

```html
<div class="logo-wordmark">
  Scholars
  <small>K-12 Management System</small>
</div>
```

Replace `Scholars` and `K-12 Management System` with your school's name and tagline.

### Changing the Accent Color
Find the `:root` CSS block near the top of the file:

```css
:root {
  --blue: #2563eb;
  --blue-light: #eff4ff;
  --blue-mid: #bfcffd;
}
```

Replace `#2563eb` with your preferred brand color (e.g., `#16a34a` for green).

### Pre-loading Your Own Student Data
Find the `students` array in the `<script>` section and replace the sample entries with your real student records following the same object format:

```javascript
const students = [
  {
    id: 'STU-001',
    name: 'First Last',
    grade: 'Grade 10',
    sec: 'A',
    phone: '555-0000',
    gpa: 3.5,
    status: 'Active',
    c: '#2563eb'   // avatar color (hex)
  },
  // ...
];
```

---

## Tech Stack

| Layer | Technology |
|---|---|
| **Structure** | HTML5 |
| **Styling** | CSS3 (custom properties, grid, flexbox, animations) |
| **Logic** | Vanilla JavaScript (ES6+) |
| **Fonts** | Google Fonts — Fraunces (display) + DM Sans (body) |
| **Icons** | Unicode emoji |
| **Dependencies** | None |
| **Bundle size** | ~1 file, ~75 KB |

---

## File Structure

```
scholars-k12-school-management.html   ← The entire application
README.md                             ← This file
```

Everything — HTML structure, CSS styles, JavaScript logic, and sample data — lives inside the single `.html` file for maximum portability.

---

## FAQ

**Q: Does this need an internet connection?**
Only for loading the Google Fonts (Fraunces + DM Sans). If offline, the app falls back to system fonts but all functionality remains.

**Q: Can I use this on a tablet or mobile?**
The layout is optimized for desktop/laptop (Windows). Tablet use is possible in landscape mode, but mobile is not currently supported.

**Q: Is data saved when I close the browser?**
No — all data is in-memory only. To persist data, you would need to add a `localStorage` layer or connect to a backend database.

**Q: How do I print the timetable or a student report?**
Use your browser's built-in print function (`Ctrl + P`). For better print results, use Chrome's "Print to PDF" option.

**Q: Can multiple admin users use this simultaneously?**
Not in the current standalone version. For multi-user access, the app would need a server backend.

**Q: How do I add more classes or subjects?**
Edit the `timetable` and `students` data objects in the `<script>` section of the HTML file with your school's actual data.

---

## License

This project is provided as-is for educational and administrative use. Customize freely for your school's needs.

---

*Built with ❤️ for K-12 schools — Scholars Management System v1.0*
