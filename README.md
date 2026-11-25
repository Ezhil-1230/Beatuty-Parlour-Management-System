# Beauty Parlour Management System (BPMS)

A full-stack web application built with **PHP**, **MySQL**, **HTML5**, **CSS3**, **JavaScript**, and **Bootstrap** to manage salon customer records, service catalogs, appointment scheduling, invoicing, and administrative reporting.

---

## Tech Stack

- **Backend:** PHP (MySQLi)
- **Database:** MySQL (`bpmsdb`)
- **Frontend:** HTML5, CSS3, JavaScript, jQuery, Bootstrap

---

## Features

### Customer Portal (`bpms/`)
- Browse salon services, about page, and contact information
- User registration, login, profile management, and password reset/change
- Online appointment booking with booking history & appointment status details
- View and print service invoices

### Admin Panel (`bpms/admin/`)
- Admin dashboard with summary metrics
- Manage services (add, edit, list)
- Review and accept/reject customer appointments
- Manage customer list, assign services, and generate invoices
- View date-range reports, sales reports, and customer enquiries

---

## Project Structure

```text
Beatuty-Parlour-Management-System-PHP/
├── bpms/
│   ├── admin/                  # Admin dashboard & management pages
│   ├── assets/                 # CSS, JS, fonts, images, and videos
│   ├── includes/               # Header, footer & DB connection
│   ├── index.php               # Customer home page
│   ├── book-appointment.php    # Appointment booking page
│   ├── login.php / signup.php  # Customer authentication
│   └── ...
├── SQL File/
│   └── bpmsdb.sql              # MySQL database schema & seed data
└── Readme.txt
```

---

## Setup & How to Run (XAMPP / WAMP)

1. Copy the `bpms/` folder into your server root (`C:\xampp\htdocs\bpms` for XAMPP or `www/bpms` for WAMP).
2. Start **Apache** and **MySQL** in XAMPP/WAMP.
3. Open **phpMyAdmin** (`http://localhost/phpmyadmin`), create a database named **`bpmsdb`**, and import **`SQL File/bpmsdb.sql`**.
4. Database settings in `bpms/includes/dbconnection.php` and `bpms/admin/includes/dbconnection.php`:
   - Host: `localhost`
   - User: `root`
   - Password: `""` (empty)
   - Database: `bpmsdb`
5. Open **`http://localhost/bpms/`** in your browser (Admin panel: `http://localhost/bpms/admin/`).

*(See `Readme.txt` for demo login credentials.)*
