# College Placement Tracker

A comprehensive Android application for managing college placement activities with role-based access for Students, HODs, and Training & Placement Officers (TPO).

Built with Kotlin and Android Jetpack.

---

## Download

[Download Latest APK](https://github.com/AnandMuliya/CollegePlacementTracker/releases/latest/download/app-debug.apk)

> Install on any Android device (Android 7.0+). Enable "Install from unknown sources" in your phone settings before installing.

---

## Screenshots

### Login

<p align="center">
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/login.jpeg" width="250" alt="Login Screen"/>
</p>

### Student View

<p align="center">
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/student_dashboard.jpeg" width="250" alt="Student Dashboard"/>
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/available_companies.jpeg" width="250" alt="Available Companies"/>
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/placement_resources.jpeg" width="250" alt="Placement Resources"/>
</p>

### TPO View

<p align="center">
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/tpo_dashboard.jpeg" width="250" alt="TPO Dashboard"/>
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/tpo_settings.jpeg" width="250" alt="TPO Settings"/>
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/interview_management.jpeg" width="250" alt="Interview Management"/>
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/schedule_interview.jpeg" width="250" alt="Schedule Interview"/>
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/reports_analysis.jpeg" width="250" alt="Reports and Analysis"/>
</p>

### HOD View

<p align="center">
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/hod_dashboard.jpeg" width="250" alt="HOD Dashboard"/>
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/all_students.jpeg" width="250" alt="All Students"/>
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/AnandMuliya/CollegePlacementTracker/main/screenshots/department_analysis.jpeg" width="250" alt="Department Analysis"/>
</p>

---

## Features

### Student
- View and search available companies with filters (package range, company type)
- Apply to eligible companies based on CGPA and branch
- Track application status in real-time
- Access placement resources (Resume Templates, Interview Tips, Coding Practice, etc.)
- View career progress and upcoming opportunities on dashboard

### TPO (Training & Placement Officer)
- Manage companies and student applications
- Schedule and manage interviews
- Generate placement reports (Overall, Student, Company, Application Status)
- View real-time placement statistics
- Configure placement settings and notifications

### HOD
- Monitor department-wise placement statistics
- View and manage students in the department
- Approve or reject student applications
- Department analysis with placement overview

---

## Getting Started

### Prerequisites
- Android Studio Hedgehog or later
- Android SDK 24+
- Kotlin 1.9.0+

### Installation

1. Clone the repository
```bash
git clone https://github.com/AnandMuliya/CollegePlacementTracker.git
```

2. Open in Android Studio

3. Let Gradle sync dependencies

4. Run the app on an emulator or physical device

---

## Project Structure

```
app/
├── src/main/
│   ├── java/com/example/collegeplacementtracker/
│   │   ├── ui/                    # UI components (Bottom Sheets, Dialogs)
│   │   ├── utils/
│   │   │   ├── SecurityUtils.kt   # Password hashing & security
│   │   │   ├── ValidationUtils.kt # Input validation
│   │   │   ├── UIHelper.kt        # UI helper methods
│   │   │   ├── DateUtils.kt       # Date formatting
│   │   │   └── NotificationHelper.kt
│   │   ├── *Activity.kt           # Activity classes
│   │   ├── *Adapter.kt            # RecyclerView adapters
│   │   ├── *Dao.kt                # Room Database DAOs
│   │   └── *.kt                   # Data models
│   └── res/
│       ├── layout/                # XML layouts
│       ├── drawable/              # Icons and images
│       └── values/                # Strings, colors, themes
```

---

## Tech Stack

| Category | Technology |
|---|---|
| Language | Kotlin |
| UI | Material Design 3 |
| Architecture | MVVM |
| Database | Room (SQLite) |
| Async | Kotlin Coroutines |
| Reactive UI | LiveData |
| Background | WorkManager |
| Charts | MPAndroidChart |
| Animations | Lottie |
| PDF Export | iTextG |

---

## Database Schema

**Users** — id, email, password, fullName, role, rollNumber, branch, cgpa

**Companies** — id, companyName, jobRole, packageAmount, location, eligibleBranches, minimumCGPA, applicationDeadline

**Applications** — id, studentId, companyId, status, currentRound, hodApproved, tpoApproved

---

## Future Enhancements

- Resume upload and parsing
- AI-powered resume analysis
- Video interview integration
- Alumni networking
- Dark mode
- Multi-language support
- Calendar sync

---

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License.

---

## Author

**Anand Muliya** — [GitHub](https://github.com/AnandMuliya)

---

Give a star if this project helped you!
