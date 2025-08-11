# 📝 PHP User Authentication System

This project is a simple **User Authentication System** built with **PHP** and **MySQL**.  
It allows users to **Sign Up**, **Log In**, and **Log Out**, with a personalized **Welcome Page**.

---

## 📂 Project Files

| File Name     | Description |
|---------------|-------------|
| `connect.php` ⚡ | Connects the project to the MySQL database. |
| `sign.php` 🆕 | Handles **user registration** (Sign Up form + backend logic). |
| `login.php` 🔐 | Handles **user login** (Login form + backend logic). |
| `home.php` 🏠 | Displays a welcome message to the logged-in user. |
| `logout.php` 🚪 | Ends the user session and redirects to the login page. |

---

## ⚙️ How It Works

1. **Database Connection** 🗄  
   `connect.php` uses `mysqli_connect()` to connect PHP to the MySQL database.

2. **User Signup** ✍  
   - `sign.php` checks if the username already exists.  
   - If not, it stores the **username** and **password** in the `registration` table.  
   - Redirects the user to `login.php` after successful signup.

3. **User Login** 🔑  
   - `login.php` verifies the entered credentials with database records.  
   - If correct, it starts a PHP session and redirects to `home.php`.

4. **Welcome Page** 🎉  
   - `home.php` greets the logged-in user by name.  
   - Provides a **Logout** button.

5. **Logout** ⏏  
   - `logout.php` destroys the session and redirects to the login page.

---

## 📊 Database Structure

**Database Name:** `signupforms`  
**Table Name:** `registration`  

| Column Name | Type          | Description |
|-------------|--------------|-------------|
| `id`        | INT (Primary Key, Auto Increment) | Unique user ID |
| `username`  | VARCHAR(255)  | Username |
| `password`  | VARCHAR(255)  | Password (stored in plain text in this project) |

---

## 🛠 Technologies Used

- **PHP** 🐘 – Server-side scripting  
- **MySQL** 🗄 – Database  
- **Bootstrap 5** 🎨 – Styling and responsive design  
- **HTML + CSS** 🌐 – Structure and basic design

---

## 📚 What You Learn from This Project

✔ How to connect PHP with MySQL using `mysqli_connect()`  
✔ How to insert and fetch data from a database  
✔ How to handle forms with the POST method  
✔ How to create sessions and manage login states  
✔ How to redirect users with `header()` in PHP  
✔ How to display Bootstrap alerts for success or error messages  

---

## 🚀 How to Run This Project

1. Install **XAMPP** or **WAMP**.  
2. Start **Apache** and **MySQL**.  
3. Create a database named `signupforms`.  
4. Create a table `registration`:

```sql
CREATE TABLE `registration` (
  `id` INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
  `username` VARCHAR(255) NOT NULL,
  `password` VARCHAR(255) NOT NULL
);
```

---

## 📧 Contact
- **LinkedIn**: [Aman Kumar](https://www.linkedin.com/in/aman-kumar-64b22b270/)
- **Portfolio**: [Visit Here](https://aman-first-portfolio.netlify.app/)

---

### 🌟 Show your support by giving this repository a ⭐!

