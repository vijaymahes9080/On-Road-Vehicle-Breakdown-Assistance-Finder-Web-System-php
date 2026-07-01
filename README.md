# 🚗 On-Road Vehicle Breakdown Assistance Finder Web System

<div align="center">

![Laravel](https://img.shields.io/badge/Laravel-6.x-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-7.2+-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-Frontend-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**A Laravel-based web application that connects stranded motorists with nearby mechanics and roadside assistance providers.**

[🔗 Live Demo](#) · [🐛 Report Bug](https://github.com/vijaymahes9080/On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php/issues) · [✨ Request Feature](https://github.com/vijaymahes9080/On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php/issues)

</div>

---

## 📌 About The Project

When a vehicle breaks down on the road, finding immediate help can be stressful and time-consuming. This web system bridges the gap between **users** who need roadside assistance and **mechanics/service providers** who can help — all from a web browser, in real time.

The platform supports three types of users:
- 👤 **Customers** – Find and request nearby mechanics
- 🔧 **Mechanics** – Accept service requests and manage their profile
- 🛡️ **Admins** – Oversee the entire platform

---

## ✨ Features

- 🔐 **Multi-Role Authentication** – Separate login/register portals for Users, Mechanics, and Admins
- 📍 **Location-Based Mechanic Search** – Find mechanics based on your breakdown location
- 🔧 **Mechanic Profiles** – Browse specializations, ratings, and real-time availability
- 📩 **Service Request System** – Submit, track, and manage breakdown requests
- 💬 **In-App Messaging** – Direct communication between customers and mechanics
- ⭐ **Feedback & Ratings** – Rate mechanics after a completed service
- 🛠️ **Admin Dashboard** – Full platform control: manage users, mechanics, and requests
- 📊 **Activity Reports** – View system usage and statistics

---

## 🛠️ Tech Stack

| Layer            | Technology                 |
|------------------|----------------------------|
| Backend Framework | Laravel 6.x               |
| Language          | PHP 7.2+                  |
| Frontend          | Blade Templates, Bootstrap |
| Database          | MySQL                      |
| Package Manager   | Composer, NPM              |
| Build Tool        | Laravel Mix / Webpack      |

---

## 📂 Project Structure

```
On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System/
├── app/
│   ├── Admin.php               # Admin model
│   ├── Mechanic.php            # Mechanic model
│   ├── User.php                # Customer model
│   ├── Feedback.php            # Feedback model
│   ├── Requests.php            # Service request model
│   ├── Messages.php            # Messaging model
│   └── Http/
│       └── Controllers/        # All route controllers
├── config/                     # App configuration files
├── database/
│   ├── migrations/             # DB schema migrations
│   └── seeds/                  # Database seeders
├── public/                     # Web-accessible assets (CSS, JS, images)
├── resources/
│   ├── views/
│   │   ├── admin/              # Admin panel views
│   │   ├── customer/           # Customer portal views
│   │   ├── mechanic/           # Mechanic portal views
│   │   ├── auth/               # Login & registration views
│   │   └── layouts/            # Shared layout templates
│   ├── js/                     # JavaScript source files
│   └── sass/                   # SCSS stylesheets
├── routes/
│   └── web.php                 # Application routes
├── SQL DATABASE/               # SQL dump for database import
├── storage/                    # Logs, cache, uploaded files
├── tests/                      # Automated tests
├── .env.example                # Environment config template
├── composer.json               # PHP dependencies
├── package.json                # Node dependencies
└── webpack.mix.js              # Asset bundling config
```

---

## ⚙️ Installation & Setup

### Prerequisites

Make sure you have the following installed:

- PHP >= 7.2
- [Composer](https://getcomposer.org/)
- MySQL / MariaDB
- Node.js & NPM

### Step-by-Step Setup

```bash
# 1. Clone the repository
git clone https://github.com/vijaymahes9080/On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php.git
cd On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php

# 2. Install PHP dependencies
composer install

# 3. Install Node.js dependencies
npm install

# 4. Copy environment config
cp .env.example .env

# 5. Generate application key
php artisan key:generate
```

### 🗄️ Database Configuration

Open `.env` and update your database credentials:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

Then import the SQL dump:

```bash
# Using MySQL CLI
mysql -u root -p your_database_name < "SQL DATABASE/vbs.sql"

# OR use phpMyAdmin to import the file from the SQL DATABASE/ folder
```

### 🚀 Run the Application

```bash
# Build frontend assets
npm run dev

# Start Laravel development server
php artisan serve
```

Visit **`http://localhost:8000`** in your browser.

---

## 👥 User Roles & Access

| Role     | Default URL         | Capabilities                              |
|----------|---------------------|-------------------------------------------|
| Customer | `/home`             | Search mechanics, submit requests, message |
| Mechanic | `/mechanic/dashboard` | Accept requests, manage profile, message |
| Admin    | `/admin/dashboard`  | Manage all users, mechanics, and requests  |

---

## 🖼️ Screenshots

> _Screenshots coming soon_

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. **Fork** this repository
2. **Create** your feature branch: `git checkout -b feature/AmazingFeature`
3. **Commit** your changes: `git commit -m 'Add AmazingFeature'`
4. **Push** to the branch: `git push origin feature/AmazingFeature`
5. **Open** a Pull Request

---

## 👤 Author

**Vijay Mahes**

- 🐙 GitHub: [@vijaymahes9080](https://github.com/vijaymahes9080)
- 📦 Repository: [On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php](https://github.com/vijaymahes9080/On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## ⚠️ Important Notes

> Never commit your `.env` file. It contains sensitive credentials.
> The `.env` file is excluded from version control by `.gitignore`.
> Always use `.env.example` as a safe template for sharing configuration.
