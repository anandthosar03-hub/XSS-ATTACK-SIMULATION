🚨 XSS Attack Demo (Educational Cybersecurity Project)
📌 Project Overview

This project demonstrates Cross-Site Scripting (XSS) vulnerabilities and their secure mitigation techniques using practical examples.

It is designed for:

Cybersecurity learners 👨‍💻
Ethical hacking students 🔐
Web security training 🛡️

The project shows:

🔴 Vulnerable implementation (unsafe input handling)
🟢 Secure implementation (input sanitization & validation)
🎯 Objectives
Understand how XSS attacks work
Demonstrate real-world XSS vulnerabilities
Learn how to fix XSS using secure coding practices
Compare vulnerable vs secure code
🛠️ Technologies Used
Frontend: HTML, CSS
Backend: PHP
Server: Python (Simple HTTP Server)
Styling: Custom CSS
📂 Project Structure
XSS-ATTACK-DEMO/
│
├── index.php                # Main entry page
├── vulnerable.php           # XSS vulnerable page
├── secure.php               # Fixed secure version
├── server.py                # Local server script
│
├── style.css                # Main styling
├── style-light.css          # Light theme
├── style_backup.css         # Backup styles
│
├── README.md                # Project documentation
├── project_handover_report.md
│
└── .git/
⚠️ XSS Vulnerability Explained
🔴 Vulnerable Code (Example)
Accepts user input directly
Outputs it without sanitization

👉 This allows attackers to inject scripts like:

<script>alert('XSS Attack')</script>
🟢 Secure Code (Fix)
Uses input sanitization methods:
htmlspecialchars() in PHP
Input validation

👉 Prevents execution of malicious scripts

🚀 How to Run the Project
Step 1: Clone Repository
git clone https://github.com/anandthosar03-hub/XSS-ATTACK-DEMO.git
cd XSS-ATTACK-DEMO
Step 2: Run Server
Option 1: Python Server
python server.py

OR

python -m http.server 8000
Step 3: Open in Browser
http://localhost:8000
🧪 How to Test XSS
Go to vulnerable page

Enter payload:

<script>alert('XSS')</script>
Observe popup → ❌ Vulnerable
Go to secure page
Enter same payload → ✅ Safe (no execution)
🔐 Security Concepts Covered
Cross-Site Scripting (XSS)
Input validation
Output encoding
Secure coding practices
Client-side vs server-side security
⚖️ Disclaimer

This project is created strictly for educational purposes only.

❗ Do NOT use these techniques on:

Real websites
Unauthorized systems

Unauthorized testing may be illegal.
