````md

MIRO LINK: https://miro.com/welcomeonboard/QnRNM0lDWko0ZzZkbkQ3eHhGRkdFeGRub1Q1ZktoWElZbTZzbFhHV0JhOXVKQitOR0NlN0NrenlFeXhQbW83Yk9aWFFpQkZBZUxCUUJEbXprblhNME4yR2padTRGVzdqKzVYSkNTWXpjM2RWVkpJT0NjcUJpR3JybitmVFF1QU9QdGo1ZEV3bUdPQWRZUHQzSGl6V2NBPT0hdjE=?share_link_id=969936020188

# TraMo – Transport Monitoring System

## Table of Contents
1. Prerequisites
2. Installation Steps
3. Running the Application
4. Helpful Tips
5. Troubleshooting

---

### 1. Prerequisites

| Tool                                 | Purpose                                        |
| ------------------------------------ | ---------------------------------------------- |
| Node.js v14+                         | Run and build the React frontend              |
| npm v6+ or Yarn                      | Download frontend packages                     |
| Composer v2+                         | Install Laravel backend packages              |
| PHP v8.1+                             | Run Laravel backend code                       |
| MySQL v8.0+                           | Store application data                          |
| Laravel v10+                          | Backend framework                              |
| XAMPP or WAMP/LAMP                     | Run Apache and MySQL locally                   |
| Postman or Thunder Client             | Test API routes                                |
| Git                                   | Download project repository                     |
| Visual Studio Code (recommended)      | Edit and view project files                    |

---

## 2. Installation Steps

### Step 1: Clone the Repository
```bash
git clone https://github.com/CHRISTIAN-GONZAGA/ITE-18-FINAL-PROJECT.git
````

### Step 2: Backend Setup

* Open the project folder
* Navigate to `/backend`

Install backend dependencies:

```bash
composer install
```

### Step 3: Create `.env` File

* Duplicate `.env.example` and rename to `.env`
* Open `.env` and update database settings:

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=tramo_db
DB_USERNAME=root
DB_PASSWORD=
```

### Step 4: Generate Laravel Key

```bash
php artisan key:generate
```

### Step 5: Run Migrations and Seeders

```bash
php artisan migrate --seed
```

### Step 6: Start Backend Server

```bash
php artisan serve
```

Backend URL: `http://127.0.0.1:8000`

### Step 7: Frontend Setup

* Navigate to `/frontend` folder
* Install frontend dependencies:

```bash
npm install
```

* Start frontend development server:

```bash
npm start
```

Frontend URL: `http://localhost:3000`

---

## 3. Running the Application

* Frontend: `http://localhost:3000`
* Backend API: `http://127.0.0.1:8000/api/v1`

Default login:

* Username: `admin`
* Password: `password123`

Access:

* Dashboard
* Vehicle Management
* TraMo Modules
* Settings and other features

---

## 4. Helpful Tips

* Keep both frontend and backend terminals open
* Do not stop servers while testing
* Restart terminal if a command fails
* Ensure MySQL is running in XAMPP/WAMP/LAMP

---

## 5. Troubleshooting

### Backend issues

* Check PHP and Composer installation

### Database errors

* Ensure `.env` database name matches MySQL

### Frontend issues

* Delete `node_modules` and reinstall:

```bash
npm install
```

### Port conflicts

* Close other applications using the same port or change the port

```
```
