Student Attendance Tracker
Prepared by: MUHAMAD FARIS AIMAN BIN MOHAMAD ROSLI (2025480948)
Prepared for: TS. DR. MOHAMAD RAHIMI BIN MOHAMAD ROSMAN
Semester: MAC 2026 – AUGUST 2026
Faculty: Faculty of Information Science, UiTM Machang, Kelantan

Project Description
This project is a functional multi-page web application interface developed for the IMS566 - Advanced Web Design Development & Content Management course at UiTM Machang. It serves as a comprehensive Student Attendance Management System, allowing administrators to track, manage, and visualize student attendance data efficiently.

The application is structured across multiple HTML files linked via standard navigation, utilizing localStorage to maintain data persistence across pages. It features a modern, dark-themed UI with a seamless user experience, fully simulated on the front-end without the need for a backend database.



File Structure
The application is separated into distinct pages based on functionality:

index.html - Authentication (Login & Student Registration)
dashboard.html - Main dashboard with data visualization and statistics
attendance.html - Daily attendance marking and management
students.html - Student list, search, and CRUD operations
announcements.html - Class updates and notice board
settings.html - User profile and password management



Features Included
1. Authentication System
Admin Login: Secure simulated login with hardcoded credentials and error feedback via toast notifications. Session state is saved to localStorage.
Student Registration: A multi-step sign-up form (Student Info → Account Setup → Review & Confirm) with live validation, password strength indicator, and input formatting. Registered accounts are stored in localStorage for subsequent logins.
2. Multi-Page Navigation & Routing
Consistent sidebar navigation across all pages using standard HTML links.
Active state highlighting on the sidebar indicating the current page.
Fully responsive design: collapses into a hamburger menu overlay on mobile devices.
Authentication guard: automatically redirects unauthenticated users to the login page.
3. Interactive Dashboard
Summary statistics cards (Total Students, Present, Absent, Attendance Rate) pulling live data from localStorage.
Line Chart: Monthly attendance vs. absence percentage trend.
Doughnut Chart: Today's attendance status breakdown.
Bar Chart: Weekly attendance comparison.
Pie Chart: Overall status distribution.
Horizontal Bar Chart: Top 10 student attendance ranking.
Activity feed and low-attendance alerts.
4. Data View Pages
Attendance Records: Data table to mark daily attendance (Hadir, Tidak Hadir, Lewat) with remarks and a "Mark All Present" feature. Data is saved to localStorage and persists across sessions.
Student List: Data table displaying enrolled students with search/filter functionality, attendance percentages, and action buttons (Edit, Delete).
5. Data Visualization
Interactive charts powered by Chart.js.
Visual progress bars for individual student attendance rates.
6. CRUD Operations
Add, edit, and delete students via modal dialogs.
Dynamic data binding that instantly updates localStorage and reflects changes across all pages.
7. UI/UX Enhancements
Toast notifications for action feedback (success, error, info).
Custom form validation with real-time error messages.
Password visibility toggle.
Global search bar that redirects to the Student List page with the query parameter.
8. Content Management & Structure
Proper metadata implementation for SEO awareness.
Structured footer containing project information, developer details, quick links, and lecturer info.
Announcement posting form and preference management page.



Instructions to Test Login
To access the main application, you can use the hardcoded Admin credentials or register a new student account.

Option 1: Admin Login (Recommended)
Launch the index.html file in your web browser.
On the login screen, enter the following credentials:
Username: admin
Password: admin123
Click the "Sign In" button.
You will be redirected to dashboard.html.
Option 2: Student Registration & Login
On the login screen, click the "Register Account" link.
Complete the 3-step registration form (Name, Student ID starting with 2025, Email, Password).
Agree to the terms and click "Register".
You will be redirected back to Login. Enter your newly created Student ID as the username and your chosen password.
Click "Sign In" to access the system.



Frameworks & Libraries Used
Tailwind CSS (v3.x): Utility-first CSS framework used for rapid, responsive UI styling and layout design.
Chart.js: JavaScript library used for rendering interactive data visualizations (Line, Doughnut, Bar, Pie, and Horizontal Bar charts) on the Dashboard.
Font Awesome (v6.5.0): Icon library used for UI elements, navigation items, and action buttons.
Google Fonts:
Space Grotesk: Used for display headings and titles.
DM Sans: Used for body text and interface elements.