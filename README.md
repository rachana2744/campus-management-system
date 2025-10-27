🎓 Campus Management System

The Campus Management System is a lightweight and user-friendly web application designed to simplify event management within a campus environment. It provides administrators with tools to create and manage campus events, while students and faculty can conveniently view upcoming activities through a dynamic calendar interface.

🚀 Features

✅ Dynamic Calendar View – Displays all campus events in an interactive calendar format.
✅ Admin Event Management – Administrators can add, update, and delete events directly from the web dashboard.
✅ Real-Time Updates – Automatically refreshes the calendar when new events are added.
✅ Responsive Design – Works seamlessly across desktops, tablets, and smartphones.
✅ MySQL Integration – All events are stored and fetched from a secure MySQL database.
✅ Error Handling – Includes server-side validation and MySQL connection checks.

🧩 Tech Stack
Layer	Technology
Frontend	HTML5, CSS3, JavaScript
Backend	PHP (Procedural)
Database	MySQL
Server	XAMPP / WAMP / LAMP Stack
⚙️ Installation & Setup

Clone the Repository

git clone https://github.com/<your-username>/campus-management-system.git
cd campus-management-system


Set Up the Database

Open phpMyAdmin and create a database named campus.

Import the provided SQL file (if included) to create tables.

Ensure your MySQL server is running.

Configure Database Connection

Open db_connect.php and verify the credentials:

$servername = "localhost";
$username = "root";
$password = "";
$dbname = "campus";


Run the Project

Place the project folder inside your local server directory (htdocs for XAMPP).

Start Apache and MySQL from the control panel.

Visit: http://localhost/campus-management-system/cal2.php

🗓️ Calendar Module (cal2.php)

The Dynamic Calendar Page (cal2.php) retrieves events from the database using AJAX and PHP.
Administrators can insert new events which instantly appear on the calendar.
If a connection issue occurs (e.g., MySQL Error 2002), the page gracefully handles the error with user feedback.

🧠 Known Issues

Occasionally, users may encounter:

Connection failed: MySQL server not responding (Error 2002)


This typically indicates temporary MySQL unavailability or a connection timeout.
We are actively investigating this issue and tracking it under #12 - MySQL Connection Failure
.

🔧 Future Enhancements

Add event categories and filters (academic, sports, cultural).

Implement login-based access control (Admin / Student).

Enable email notifications for new events.

Add event search and tagging features.

Migrate to MVC structure or Laravel framework for scalability.
