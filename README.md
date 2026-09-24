# Eduflex 🎓 - Online Learning Management System

[![PHP Version](https://img.shields.io/badge/PHP-%3E%3D%207.x-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![CodeIgniter](https://img.shields.io/badge/CodeIgniter-3.x-EF4223?style=for-the-badge&logo=codeigniter&logoColor=white)](https://codeigniter.com/)
[![MySQL](https://img.shields.io/badge/MySQL-5.7%2B%20%2F%208.x-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

**Eduflex** is a full-featured, dynamic Online Learning Management System (LMS) built on the CodeIgniter PHP framework. It empowers educators to create and sell online courses while providing students with an engaging, interactive learning environment.

---

## ✨ Features

### 🎓 Student Experience
- **Course Marketplace:** Browse courses with category filtering, search, and detailed ratings.
- **Interactive Player:** Seamless video lesson playback supporting YouTube, Vimeo, and self-hosted HTML5 videos.
- **Wishlist & Cart:** Easily save favorite courses and purchase multiple courses with multi-currency support.
- **Student Dashboard:** Track enrolled courses, learning progress, and account profile settings.

### 👨‍🏫 Instructor Management
- **Course Builder:** Manage course sections, upload video lessons, set prices, and write course descriptions.
- **Revenue Dashboard:** Monitor earnings, commission breakdowns, and payout history.

### ⚙️ Admin Control Panel
- **User Management:** Control roles and permissions for Students, Instructors, and Administrators.
- **Category & Taxonomy:** Unlimited nested course categories and subcategories.
- **Financial & Payment Settings:** Configure global currencies, commission rates, and payment gateways.
- **System Customization:** Manage site titles, logos, banners, SMTP email, and system settings.

### 💳 Payment Gateways
- Integrated **Stripe** and **PayPal** checkout for secure transactions.

---

## 🛠️ Tech Stack

- **Backend:** PHP 7.x/8.x (CodeIgniter 3 MVC Framework)
- **Database:** MySQL / MariaDB
- **Frontend:** HTML5, CSS3, JavaScript, jQuery, Bootstrap, FontAwesome
- **Integrations:** PayPal REST API, Stripe PHP SDK, YouTube API, Vimeo API

---

## 🚀 Getting Started

Follow these steps to set up Eduflex locally using **XAMPP**, **WAMP**, or any standard PHP local server environment.

### Prerequisites

- [XAMPP](https://www.apachefriends.org/) (with Apache & MySQL) or equivalent local web server
- PHP 7.4+ with `curl`, `json`, `mbstring`, and `pdo_mysql` extensions enabled
- MySQL 5.7+ / MariaDB

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/neerajajoshi/Eduflex.git
   ```

2. **Move to Web Server Root**
   - Copy or move the `Eduflex` project directory into your web server's root directory:
     - **XAMPP:** `C:\xampp\htdocs\Eduflex`
     - **WAMP:** `C:\wamp64\www\Eduflex`
     - **LAMP/Linux:** `/var/www/html/Eduflex`

3. **Set Up Database**
   - Open phpMyAdmin (`http://localhost/phpmyadmin`).
   - Create a new database named `dblms`.
   - Import the database schema from [`db/dblms.sql`](file:///c:/Users/neera/Downloads/Online_Learning_Management_System/Online_Learning_Management_System/db/dblms.sql).

4. **Configure Database Connection**
   - Open [`application/config/database.php`](file:///c:/Users/neera/Downloads/Online_Learning_Management_System/Online_Learning_Management_System/application/config/database.php) and update your database credentials if needed:
     ```php
     'hostname' => 'localhost',
     'username' => 'root',
     'password' => '',
     'database' => 'dblms',
     'dbdriver' => 'mysqli',
     ```

5. **Run the Application**
   - Navigate to `http://localhost/Eduflex` in your web browser.

---

## 🔑 Default Login Credentials

After importing the database, you can log in with the following default administrator credentials:

| Role | Email | Password |
| :--- | :--- | :--- |
| **Admin** | `admin@example.com` | `admin` |

> [!IMPORTANT]
> Please change default passwords immediately after logging into your production environment!

---

## 📁 Repository Structure

```
Eduflex/
├── application/         # Core application code (Controllers, Models, Views, Libraries)
│   ├── config/          # Application configuration files
│   ├── controllers/     # Route handlers (Admin, Home, User, Login)
│   ├── models/          # Database queries & business logic
│   └── views/           # UI templates & frontend views
├── assets/              # Static assets (CSS, JS, Fonts, Images, Plugins)
├── db/                  # SQL database dump files (dblms.sql)
├── system/              # CodeIgniter 3 core framework files
├── uploads/             # Course thumbnails, user avatars & media attachments
└── index.php            # Main application entry point
```

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
