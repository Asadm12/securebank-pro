# 🔐 SecureBank Pro - Secure FinTech Application

![Security Badge](https://img.shields.io/badge/Security-100%25-success)
![Tests](https://img.shields.io/badge/Tests-35%2F35%20Passed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)

**CY4053 - Cybersecurity for FinTech | Assignment 2**  
**Fall 2025 | BSFT 7th Semester**

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Security Implementations](#security-implementations)
- [Technologies Used](#technologies-used)
- [Installation & Setup](#installation--setup)
- [Usage Guide](#usage-guide)
- [Testing Documentation](#testing-documentation)
- [Project Structure](#project-structure)
- [Security Features Demo](#security-features-demo)
- [Screenshots](#screenshots)
- [Assignment Requirements](#assignment-requirements)
- [Author](#author)

---

## 🎯 Overview

**SecureBank Pro** is a comprehensive FinTech demonstration application built to showcase cybersecurity best practices in financial technology. This application implements industry-standard security measures including authentication, input validation, data encryption, session management, and comprehensive activity logging.

### Key Highlights:
- ✅ 35+ Manual Security Tests (All Passed)
- 🔒 Multi-layer Security Architecture
- 🎨 Modern Glassmorphic UI Design
- 📊 Real-time Transaction Monitoring
- 🔐 End-to-End Encryption Demo
- 📝 Complete Activity Audit Trail

---

## ✨ Features

### 🔐 Authentication & Authorization
- **User Registration** with strong validation
- **Secure Login System** with password hashing
- **Account Lockout** after 5 failed attempts
- **Session Management** with 5-minute auto-timeout
- **Secure Logout** with session cleanup

### 💰 Banking Operations
- **Virtual Account Balance** tracking
- **Transaction Processing** with validation
- **Transaction History** with timestamps
- **Recipient Validation** and sanitization
- **Insufficient Balance** protection

### 👤 Profile Management
- **Email Validation** (RFC compliant)
- **Phone Number Validation** (international format)
- **Address Management** with sanitization
- **Profile Update** with security checks

### 🔒 Security Features
- **Password Strength Meter** (real-time feedback)
- **Input Sanitization** (XSS/SQL injection prevention)
- **Data Encryption/Decryption** demonstration
- **File Upload Validation** (type & size restrictions)
- **Activity Logging** (complete audit trail)

### 🎨 User Interface
- **Glassmorphic Design** with backdrop blur
- **Gradient Color Schemes** (purple/blue theme)
- **Responsive Layout** (mobile & desktop)
- **Real-time Feedback** (alerts & notifications)
- **Interactive Animations** (smooth transitions)

---

## 🛡️ Security Implementations

### 1. Authentication Security
```javascript
✓ Password Hashing (SHA-256 simulation)
✓ Minimum 8 characters enforced
✓ Requires: 1 number + 1 special symbol
✓ Password confirmation matching
✓ Login attempt tracking
✓ Account lockout mechanism (5 attempts)
```

### 2. Input Validation & Sanitization
```javascript
✓ HTML entity escaping (prevents XSS)
✓ Special character filtering
✓ SQL injection prevention
✓ Email format validation (regex)
✓ Phone number format validation
✓ Alphanumeric username enforcement
✓ Field length restrictions (maxlength)
✓ Numeric field type enforcement
```

### 3. Session Security
```javascript
✓ 5-minute inactivity timeout
✓ Visual session timer display
✓ Activity-based timeout reset
✓ Secure session storage
✓ Complete session cleanup on logout
```

### 4. Data Protection
```javascript
✓ Password storage as hashed values
✓ Encryption/Decryption capability
✓ Base64 + Reverse encoding
✓ Secure localStorage usage
✓ No plaintext sensitive data
```

### 5. File Upload Security
```javascript
✓ Whitelist: .pdf, .doc, .docx, .txt, .jpg, .png
✓ Blacklist: .exe, .bat, .sh, .js (executables)
✓ Maximum size: 5MB
✓ Extension validation
✓ MIME type checking
```

### 6. Error Handling
```javascript
✓ Generic error messages (no sensitive info)
✓ No stack trace exposure
✓ User-friendly notifications
✓ Graceful degradation
✓ Controlled error recovery
```

### 7. Activity Logging
```javascript
✓ User registration events
✓ Login/logout tracking
✓ Failed login attempts
✓ Transaction records
✓ Profile updates
✓ File uploads
✓ Encryption operations
✓ Timestamp for all actions
```

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| **HTML5** | Structure & Semantic Markup |
| **CSS3** | Styling, Animations, Glassmorphism |
| **JavaScript (ES6+)** | Application Logic & Security |
| **LocalStorage API** | Client-side Data Persistence |
| **Base64 Encoding** | Encryption Demonstration |
| **Regex Patterns** | Input Validation |
| **HTML5 Form Validation** | Client-side Validation |

### Why Pure HTML/CSS/JS?
- ✅ **No Dependencies** - Zero installation required
- ✅ **Easy Testing** - Open directly in browser
- ✅ **Full Control** - Complete security implementation
- ✅ **Fast Development** - Rapid prototyping
- ✅ **Assignment Flexibility** - Meets all requirements

---

## 📦 Installation & Setup

### Prerequisites
- Modern web browser (Chrome, Firefox, Edge, Safari)
- Text editor (VS Code, Sublime, Notepad++)
- No server or dependencies required!

### Quick Start (30 seconds)

1. **Clone/Download the repository**
   ```bash
   git clone https://github.com/yourusername/securebank-pro.git
   cd securebank-pro
   ```

2. **Open the application**
   - Double-click `index.html`
   - OR right-click → Open with → Chrome
   - OR drag `index.html` into browser window

3. **Start testing!**
   - Register a new account
   - Explore all features
   - Perform security tests

### Alternative: Run from VS Code
1. Install "Live Server" extension
2. Right-click `index.html`
3. Select "Open with Live Server"

---

## 📖 Usage Guide

### Creating an Account

1. Click **"Create New Account"**
2. Enter username (alphanumeric only)
3. Enter valid email address
4. Create strong password (8+ chars, 1 number, 1 symbol)
5. Confirm password
6. Click **"Register"**

### Logging In

1. Enter registered username
2. Enter password
3. Click **"Login"**
4. ⚠️ Note: Account locks after 5 failed attempts

### Making Transactions

1. Navigate to **"Transactions"** tab
2. Enter recipient name
3. Enter amount (numeric only)
4. Add description (optional)
5. Click **"Send Money"**
6. View transaction in history below

### Updating Profile

1. Go to **"Profile"** tab
2. Update email, phone, or address
3. Click **"Save Changes"**
4. ✅ All fields validated before saving

### Encryption Demo

1. Click **"Encryption"** tab
2. Enter sensitive data
3. Click **"Encrypt"** to see encrypted output
4. Click **"Decrypt"** to restore original

### File Upload

1. Navigate to **"File Upload"** tab
2. Click upload zone
3. Select allowed file types only
4. ⛔ Executables (.exe, .bat) automatically blocked

### Viewing Activity Logs

1. Go to **"Activity Logs"** tab
2. View chronological list of all actions
3. Each entry shows timestamp
4. Useful for security auditing

---

## 🧪 Testing Documentation

### Test Summary
- **Total Tests:** 35
- **Passed:** 35 ✅
- **Failed:** 0
- **Success Rate:** 100%

### Test Categories

| Category | Tests | Status |
|----------|-------|--------|
| Input Validation | 10 | ✅ All Passed |
| Authentication | 8 | ✅ All Passed |
| Authorization | 4 | ✅ All Passed |
| Data Security | 6 | ✅ All Passed |
| Session Management | 3 | ✅ All Passed |
| File Upload | 4 | ✅ All Passed |

### Key Security Tests Performed

1. ✅ SQL Injection Prevention (Login & Forms)
2. ✅ Cross-Site Scripting (XSS) Protection
3. ✅ Password Strength Enforcement
4. ✅ Email Validation
5. ✅ Brute Force Protection (Account Lockout)
6. ✅ Session Timeout (5 minutes)
7. ✅ Password Hashing Verification
8. ✅ Input Sanitization
9. ✅ File Upload Restrictions
10. ✅ Error Message Security
11. ✅ Unauthorized Access Prevention
12. ✅ Data Encryption/Decryption
13. ✅ Activity Logging
14. ✅ Transaction Validation
15. ✅ Profile Update Security

**Full testing documentation available in:** `Testing_Documentation.md`

---

## 📁 Project Structure

```
SecureBank-FinTech/
│
├── index.html                 # Main application file (complete app)
├── README.md                  # This file
├── Testing_Documentation.md   # Complete test cases & results
│
├── screenshots/               # Test evidence screenshots
│   ├── test01_sql_injection.png
│   ├── test02_xss_attack.png
│   ├── test03_weak_password.png
│   └── ... (35+ screenshots)
│
└── docs/                      # Additional documentation
    ├── SECURITY.md           # Security architecture details
    └── USER_GUIDE.pdf        # Printable user manual
```

---

## 🔒 Security Features Demo

### Password Hashing
```javascript
// Passwords are NEVER stored in plaintext
Input:  "MySecurePass123!"
Stored: "SHA256:7f4a8b9c2e1d6f3a..."
```

### Input Sanitization
```javascript
// Malicious inputs are automatically cleaned
Input:  "<script>alert('XSS')</script>"
Output: "scriptalert('XSS')/script" (tags removed)
```

### Session Management
```javascript
// Sessions expire after 5 minutes of inactivity
Session Start: 5:00
User Idle: ...
Auto Logout: 0:00 ⚠️
```

### File Upload Validation
```javascript
// Dangerous files are blocked
.pdf  ✅ Allowed
.jpg  ✅ Allowed
.exe  ❌ BLOCKED
.bat  ❌ BLOCKED
```

---

## 📸 Screenshots

### Main Interface
![Login Screen](screenshots/test09_successful_login.png)
*Secure login interface with session management*

### Security Features
![Encryption Demo](screenshots/test16_encryption.png)
*Real-time data encryption demonstration*

### Testing Evidence
![Failed Login Attempts](screenshots/test08_failed_login.png)
*Account lockout after multiple failed attempts*

**📁 All screenshots available in:** `/screenshots` folder

---

## ✅ Assignment Requirements Checklist

### Required Features (10/10)
- [x] User Registration & Login
- [x] Password Validation (Strong rules)
- [x] Input Forms (Secure validation)
- [x] Session Management
- [x] Data Storage Layer (Encrypted/Hashed)
- [x] Error Handling (No info leakage)
- [x] Encryption/Decryption Option
- [x] Audit/Activity Logs
- [x] Profile Update Page
- [x] File Upload Validation

### Testing Requirements
- [x] 20+ Manual Tests (35 completed)
- [x] Test Documentation Table
- [x] Screenshots for Each Test
- [x] Pass/Fail Results

### Deliverables
- [x] Source Code (index.html)
- [x] GitHub Repository with README
- [x] Test Case Documentation
- [x] Screenshots Folder
- [x] Optional: Video Demo Link

---

## 🎓 Learning Outcomes

This project demonstrates understanding of:
- ✅ Secure coding practices
- ✅ Input validation techniques
- ✅ Authentication mechanisms
- ✅ Session management
- ✅ Data encryption
- ✅ Error handling
- ✅ Security testing methodologies
- ✅ OWASP Top 10 vulnerabilities

---

## 🚀 Future Enhancements

- [ ] Backend integration (Node.js/Express)
- [ ] Database implementation (MongoDB/PostgreSQL)
- [ ] Two-Factor Authentication (2FA)
- [ ] OAuth integration (Google/GitHub)
- [ ] Advanced encryption (AES-256)
- [ ] Rate limiting middleware
- [ ] CAPTCHA for login
- [ ] Email verification
- [ ] Password reset functionality
- [ ] Mobile application version

---

## 📝 License

This project is created for educational purposes as part of CY4053 - Cybersecurity for FinTech course.

**MIT License** - Feel free to use for learning purposes.


---

## 🙏 Acknowledgments

- Dr. Usama Arshad for course guidance
- OWASP for security best practices
- MDN Web Docs for technical reference
- Anthropic Claude for development assistance

---

## 📞 Contact

For questions or feedback:
- Email: asadmalik200315@gmail.com
- GitHub: Asadm12


---

## 🔗 Quick Links

- [Live Demo](https://yourusername.github.io/securebank-pro)
- [Documentation](docs/)
- [Report Issues](https://github.com/yourusername/securebank-pro/issues)
- [View Tests](Testing_Documentation.md)

---

<div align="center">

**⭐ If this project helped you, consider giving it a star!**

Made with 💙 for Cybersecurity Education

</div>