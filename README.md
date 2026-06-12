# Admin Authentication Dashboard (Frontend Only)

A simple **frontend authentication system** built using **HTML, Tailwind CSS, and JavaScript**.  
It includes Signup, Login, and a protected Dashboard using **LocalStorage** for authentication.

---

## 🚀 Features

- User Signup with form validation
- Login system using LocalStorage
- Email and password validation
- Password confirmation check
- Protected Dashboard (redirect if not logged in)
- Logout functionality
- Display logged-in user name
- Fetch and display users from FakeStore API
- Responsive UI using Tailwind CSS



## 🧠 How It Works

### 🔹 Signup Page
- User fills form (first name, last name, email, password)
- Validation is applied:
  - All fields required
  - Valid email format
  - Password must be 8+ characters with number
  - Confirm password must match
- Data is stored in **localStorage**
- Redirects to Login page

---

### 🔹 Login Page
- User enters email and password
- Data is checked from **localStorage**
- If correct:
  - `isLoggedIn = true`
  - Redirect to Dashboard
- If incorrect → error message shown

---

### 🔹 Dashboard Page
- Only accessible if user is logged in
- Otherwise redirects to Login page
- Shows logged-in user name
- Displays total users fetched from API
- Shows users in a table

---

## 🔐 Authentication Logic
- Data stored in localStorage under key user
- Login state managed using:
  isLoggedIn: true