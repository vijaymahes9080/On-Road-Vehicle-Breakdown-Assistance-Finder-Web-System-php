# 🚗 On-Road Vehicle Breakdown Assistance Finder Web System

A **Laravel-based web application** that connects stranded motorists with nearby mechanics and roadside assistance providers in real time.

---

## 📌 Project Overview

When a vehicle breaks down on the road, finding immediate help can be stressful. This system bridges the gap between **users** who need roadside assistance and **mechanics/service providers** who can help — all from a web browser.

---

## ✨ Features

- 🔐 **User Registration & Login** – Separate portals for Users, Mechanics, and Admins
- 📍 **Location-Based Search** – Find nearby mechanics based on breakdown location
- 🔧 **Mechanic Profiles** – Browse mechanic specializations, ratings, and availability
- 📩 **Service Requests** – Users can submit breakdown requests to mechanics
- 💬 **Messaging System** – In-app communication between users and mechanics
- ⭐ **Feedback & Ratings** – Rate mechanics after service completion
- 🛠️ **Admin Dashboard** – Manage users, mechanics, and service requests
- 📊 **Reports** – View system activity and statistics

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend Framework | Laravel 6.x |
| Language | PHP 7.2+ |
| Frontend | Blade Templates, Bootstrap |
| Database | MySQL |
| Package Manager | Composer, NPM |
| Build Tool | Laravel Mix / Webpack |

---

## 📂 Project Structure

```
On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System/
├── app/                    # Core application (Models, Controllers, Middleware)
│   ├── Admin.php           # Admin model
│   ├── Mechanic.php        # Mechanic model
│   ├── User.php            # User model
│   ├── Feedback.php        # Feedback model
│   ├── Requests.php        # Service request model
│   └── Http/               # Controllers & Middleware
├── config/                 # Configuration files
├── database/               # Migrations, Seeders, Factories
├── public/                 # Publicly accessible assets
├── resources/              # Views, CSS, JS sources
│   └── views/              # Blade templates
├── routes/                 # Web & API route definitions
├── SQL DATABASE/           # SQL dump file for database setup
├── storage/                # Logs, cache, uploaded files
└── tests/                  # Automated tests
```

---

## ⚙️ Installation & Setup

### Prerequisites
- PHP >= 7.2
- Composer
- MySQL
- Node.js & NPM

### Steps

```bash
# 1. Clone the repository
git clone https://github.com/vijaymahes9080/On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php.git
cd On-Road-Vehicle-Breakdown-Assistance-Finder-Web-System-php

# 2. Install PHP dependencies
composer install

# 3. Install Node dependencies
npm install

# 4. Copy and configure environment file
cp .env.example .env

# 5. Generate application key
php artisan key:generate

# 6. Configure your database in .env
# DB_DATABASE=your_database_name
# DB_USERNAME=your_username
# DB_PASSWORD=your_password

# 7. Import the SQL database
# Import the file from the SQL DATABASE/ folder using phpMyAdmin or MySQL CLI:
# mysql -u root -p your_database_name < "SQL DATABASE/your_dump.sql"

# 8. Run database migrations (if applicable)
php artisan migrate

# 9. Build frontend assets
npm run dev

# 10. Start the development server
php artisan serve
```

Visit `http://localhost:8000` in your browser.

---

## 🗄️ Database Setup

The SQL dump file is located in the **`SQL DATABASE/`** folder. Import it into your MySQL server before running the application.

---

## 👤 Author

**Vijay Mahes**  
🔗 GitHub: [@vijaymahes9080](https://github.com/vijaymahes9080)

---

## 📄 License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to open an issue or submit a pull request.

---

> ⚠️ **Note**: Make sure to configure your `.env` file properly before running the application. Never commit sensitive credentials to version control.
