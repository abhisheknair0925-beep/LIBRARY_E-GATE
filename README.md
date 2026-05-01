# LIBRARY E-GATE

Library E-Gate is a web-based application designed to manage and track the check-in and check-out times of students and instructors at a library. It was initially developed for Amrita School of Arts and Science College in Kochi.

The system allows users to simply scan their ID cards upon entering and exiting the library. Based on this scan data, the application calculates the total time spent in the library and provides comprehensive tools for librarians to generate monthly or semester-by-semester reports.

## Features

- **Automated Check-in/Check-out:** Users scan their ID card (barcode/RFID) to log their entry and exit times automatically.
- **Duration Tracking:** The system calculates the exact duration of each library visit.
- **Admin Dashboard:** A secure login for librarians to access various management modules.
- **Logs Management:** View detailed logs of all student and teacher entries.
- **Statistics & Analytics:** Visual representations and statistical data regarding library usage.
- **Report Generation:** Generate detailed reports (monthly, semesterly, or custom date ranges) based on user activity.
- **Data Management:** Add, update, or remove student/staff records from the database.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript (jQuery), Bootstrap (for styling), Lottie (for animations)
- **Backend:** PHP
- **Database:** MySQL

## Getting Started

### Prerequisites

- A local server environment like XAMPP, WAMP, or MAMP.
- A barcode or RFID scanner (configured to send a carriage return / "Enter" keystroke after scanning).

### Installation

1. Clone the repository to your local server's document root (e.g., `htdocs` for XAMPP).
2. Start the Apache and MySQL services.
3. Open phpMyAdmin (usually `http://localhost/phpmyadmin`) and create a new database named `db_library`.
4. Import the provided SQL dump file (`db_library 3.sql`) into the newly created database.
5. Open your web browser and navigate to the project directory:
   - For the Admin Login: `http://localhost/LIBRARY_E-GATE/index.php` (Default password is 'amma').
   - For the E-Gate Scanner Interface: `http://localhost/LIBRARY_E-GATE/scannerindex.php`.

## Project Structure

- `scannerindex.php`: The main entry point for users to scan their IDs.
- `index.php`: Admin login page.
- `home.php`: The main dashboard for administrators.
- `db_library 3.sql`: Database schema and sample data.
- `/css`: Various stylesheets used across the application.
- Other PHP files handle specific features like reporting, stats, logs, and database updates.
