# 🚨 XSS Attack Demo (Educational Cybersecurity Project)

## 📌 Project Overview

This project demonstrates **Cross-Site Scripting (XSS)** vulnerabilities and their **secure mitigation techniques** using practical examples.

It is designed for:

* Cybersecurity learners 👨‍💻
* Ethical hacking students 🔐
* Web security training 🛡️

The project includes:

* 🔴 Vulnerable implementation (unsafe input handling)
* 🟢 Secure implementation (input sanitization & validation)

---

## 🎯 Objectives

* Understand how XSS attacks work
* Demonstrate real-world XSS vulnerabilities
* Learn how to fix XSS using secure coding practices
* Compare vulnerable vs secure code

---

## 🛠️ Technologies Used

* **Frontend:** HTML, CSS
* **Backend:** PHP
* **Server:** Python (Local server)
* **Styling:** Custom CSS

---

## 📂 Project Structure

```
XSS-ATTACK-DEMO/
│
├── index.php
├── vulnerable.php
├── secure.php
├── server.py
│
├── style.css
├── style-light.css
├── style_backup.css
│
├── README.md
├── project_handover_report.md
│
└── .git/
```

---

## ⚠️ XSS Vulnerability Explained

### 🔴 Vulnerable Example

The vulnerable page directly reflects user input without sanitization.

Example payload:

```html
<script>alert('XSS Attack')</script>
```

👉 This executes JavaScript in the browser.

---

### 🟢 Secure Implementation

The secure page uses proper sanitization:

```php
htmlspecialchars($input, ENT_QUOTES, 'UTF-8');
```

👉 Prevents execution of malicious scripts.

---

## 🚀 How to Run the Project

### 1. Clone Repository

```
git clone https://github.com/anandthosar03-hub/XSS-ATTACK-DEMO.git
cd XSS-ATTACK-DEMO
```

---

### 2. Start Server

Using Python:

```
python server.py
```

OR:

```
python -m http.server 8000
```

---

### 3. Open in Browser

```
http://localhost:8000
```

---

## 🧪 Testing the Attack

1. Open **vulnerable.php**
2. Enter:

```
<script>alert('XSS')</script>
```

➡️ Popup appears → ❌ Vulnerable

3. Open **secure.php**
   ➡️ Script is not executed → ✅ Secure

---

## 🔐 Security Concepts Covered

* Cross-Site Scripting (XSS)
* Input validation
* Output encoding
* Secure coding practices
* Web application security basics

---

## ⚖️ Disclaimer

This project is for **educational purposes only**.

❗ Do NOT use on real systems without permission
❗ Unauthorized testing is illegal

---

## ⭐ Support

If you like this project:

* ⭐ Star the repository
* 🍴 Fork it
* 🛠️ Contribute

