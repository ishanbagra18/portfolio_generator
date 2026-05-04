<div align="center">

<img src="ss3.png" alt="ProFolio Banner" width="100%"/>

<br/><br/>

# 🚀 ProFolio — Portfolio Generator with OTP Authentication

**Sign up. Verify. Build your dream portfolio — in minutes.**

[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Nodemailer](https://img.shields.io/badge/Nodemailer-0A7BBB?style=for-the-badge&logo=gmail&logoColor=white)](https://nodemailer.com/)
[![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=twilio&logoColor=white)](https://www.twilio.com/)

<br/>

![GitHub stars](https://img.shields.io/github/stars/yourusername/profolio?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/profolio?style=social)
![GitHub issues](https://img.shields.io/github/issues/yourusername/profolio?color=red)
![License](https://img.shields.io/badge/license-MIT-green)

<br/>

> 🔐 **Passwordless Auth** &nbsp;·&nbsp; ⚡ **Instant Portfolio** &nbsp;·&nbsp; 🎨 **Dark Theme UI** &nbsp;·&nbsp; 📱 **Fully Responsive**

</div>

---

## 📋 Table of Contents

- [✨ Overview](#-overview)
- [📸 Screenshots](#-screenshots)
- [🎯 Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ Installation](#️-installation)
- [🔧 Configuration](#-configuration)
- [🚀 Running the App](#-running-the-app)
- [📌 API Endpoints](#-api-endpoints)
- [🌐 Portfolio Fields](#-portfolio-fields)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Overview

**ProFolio** is a full-stack web application that lets users register, authenticate via OTP (email or SMS), fill in their professional details, and instantly generate a stunning personal portfolio website — no coding required.

```
Sign Up → OTP Verification → Dashboard → Fill Details → Portfolio Generated! 🎉
```

---

## 📸 Screenshots

### 🔐 Authentication

<table>
  <tr>
    <td align="center"><b>Login Page</b></td>
    <td align="center"><b>OTP Verification</b></td>
  </tr>
  <tr>
    <td><img src="ss1.png" alt="Login Page" width="100%"/></td>
    <td><img src="ss2.png" alt="OTP Verification" width="100%"/></td>
  </tr>
</table>

---

### 🏠 Dashboard & Portfolio Builder

<table>
  <tr>
    <td align="center"><b>Welcome Dashboard</b></td>
    <td align="center"><b>Fill Portfolio Details</b></td>
  </tr>
  <tr>
    <td><img src="ss3.png" alt="Dashboard" width="100%"/></td>
    <td><img src="ss4.png" alt="Portfolio Form" width="100%"/></td>
  </tr>
</table>

<table>
  <tr>
    <td align="center"><b>AI Features Overview</b></td>
    <td align="center"><b>Competitive Programming Profiles</b></td>
  </tr>
  <tr>
    <td><img src="ss5.png" alt="Features" width="100%"/></td>
    <td><img src="ss6.png" alt="Coding Profiles" width="100%"/></td>
  </tr>
</table>

<table>
  <tr>
    <td align="center" colspan="2"><b>Portfolio Saved Successfully ✅</b></td>
  </tr>
  <tr>
    <td colspan="2" align="center"><img src="ss7.png" alt="Portfolio Saved" width="70%"/></td>
  </tr>
</table>

---

### 🎨 Generated Portfolio Output

<table>
  <tr>
    <td align="center" colspan="2"><b>Hero Section</b></td>
  </tr>
  <tr>
    <td colspan="2"><img src="ss8.png" alt="Portfolio Hero" width="100%"/></td>
  </tr>
</table>

<table>
  <tr>
    <td align="center"><b>About Me</b></td>
    <td align="center"><b>My Skills</b></td>
  </tr>
  <tr>
    <td><img src="ss9.png" alt="About Me Section" width="100%"/></td>
    <td><img src="ss10.png" alt="Skills Section" width="100%"/></td>
  </tr>
</table>

<table>
  <tr>
    <td align="center"><b>Education & Projects</b></td>
    <td align="center"><b>Competitive Coding Profiles</b></td>
  </tr>
  <tr>
    <td><img src="ss11.png" alt="Education & Projects" width="100%"/></td>
    <td><img src="ss12.png" alt="Coding Profiles Portfolio" width="100%"/></td>
  </tr>
</table>

<table>
  <tr>
    <td align="center" colspan="2"><b>Contact Section</b></td>
  </tr>
  <tr>
    <td colspan="2"><img src="ss13.png" alt="Contact Section" width="100%"/></td>
  </tr>
</table>

---

## 🎯 Features

### 🔑 Authentication
- ✅ Sign up with **email** or **phone number**
- ✅ Passwordless login via **5-digit OTP**
- ✅ OTP delivery via **Nodemailer** (email) and **Twilio** (SMS)
- ✅ OTP auto-expires and is single-use
- ✅ Secure sessions with **JWT**

### 🧑‍💼 Portfolio Builder
- ✅ Personal Info — Name, Age, Email, Phone, Address, Language
- ✅ Skills with **animated circular progress indicators**
- ✅ Education timeline (School → College → University)
- ✅ Projects with GitHub repository links
- ✅ Competitive Programming — LeetCode & CodeChef ratings
- ✅ Contact form with social links (GitHub, LinkedIn, Instagram, Email)
- ✅ Beautiful **dark-themed generated portfolio**

### 🤖 AI-Powered Capabilities
- ✅ Instant Portfolio Creation
- ✅ Customizable Templates
- ✅ AI-Optimized Content Suggestions
- ✅ Easy File Integration
- ✅ SEO & Visibility Boost
- ✅ Auto-Save & Backup
- ✅ Analytics & Insights
- ✅ Multi-Device Access

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|-----------|---------|
| HTML5 / CSS3 | Markup & Styling |
| JavaScript (ES6+) | Client-side interactivity |
| React / Vite | Component-based UI |

### Backend
| Technology | Purpose |
|-----------|---------|
| **Node.js** | Runtime environment |
| **Express.js** | Web framework & REST API |
| **JWT** | Secure session tokens |

### OTP / Messaging
| Service | Purpose |
|--------|---------|
| **Nodemailer** | Email OTP via Gmail SMTP |
| **Twilio** | SMS OTP |

### Database
| Technology | Purpose |
|-----------|---------|
| **MongoDB** | User data, sessions, portfolios |
| **Mongoose** | ODM & schema modeling |

---

## 📁 Project Structure

```
profolio/
│
├── 📂 backend/
│   ├── 📂 config/
│   │   ├── db.js                  # MongoDB connection
│   │   └── nodemailer.js          # Email transport setup
│   ├── 📂 controllers/
│   │   ├── authController.js      # Signup, OTP send/verify
│   │   └── portfolioController.js # Create, update, fetch portfolio
│   ├── 📂 middleware/
│   │   ├── authMiddleware.js      # JWT verification
│   │   └── rateLimiter.js         # OTP rate limiting
│   ├── 📂 models/
│   │   ├── User.js                # User schema
│   │   ├── OTP.js                 # OTP schema (hashed + expiry)
│   │   └── Portfolio.js           # Full portfolio schema
│   ├── 📂 routes/
│   │   ├── authRoutes.js          # /api/auth/*
│   │   └── portfolioRoutes.js     # /api/portfolio/*
│   ├── 📂 services/
│   │   ├── emailService.js        # Nodemailer OTP sender
│   │   └── smsService.js          # Twilio OTP sender
│   ├── .env
│   ├── server.js
│   └── package.json
│
├── 📂 frontend/
│   ├── 📂 src/
│   │   ├── 📂 pages/
│   │   │   ├── Login.jsx
│   │   │   ├── OTPVerify.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── PortfolioForm.jsx
│   │   │   └── Portfolio.jsx      # Generated portfolio output
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── vite.config.js
│   └── package.json
│
└── README.md
```

---

## ⚙️ Installation

### Prerequisites

- [Node.js](https://nodejs.org/) v16+
- [MongoDB](https://www.mongodb.com/) (local or Atlas)
- [Twilio](https://www.twilio.com/) account
- Gmail / SMTP credentials

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/profolio.git
cd profolio
```

### 2. Install Dependencies

```bash
# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

---

## 🔧 Configuration

Create a `.env` file in `/backend`:

```env
# ── Server ───────────────────────────────────────
PORT=5000
NODE_ENV=development

# ── Database ─────────────────────────────────────
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/profolio_db

# ── JWT ──────────────────────────────────────────
JWT_SECRET=your_super_secret_jwt_key
JWT_EXPIRES_IN=7d

# ── OTP Settings ─────────────────────────────────
OTP_EXPIRY_MINUTES=10
OTP_LENGTH=5

# ── Nodemailer (Email OTP) ────────────────────────
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_gmail_app_password

# ── Twilio (SMS OTP) ─────────────────────────────
TWILIO_ACCOUNT_SID=ACxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_PHONE_NUMBER=+1234567890
```

> ⚠️ Never commit `.env` to Git — add it to `.gitignore`.

---

## 🚀 Running the App

```bash
# Terminal 1 — Backend (http://localhost:5000)
cd backend
npm run dev

# Terminal 2 — Frontend (http://localhost:5173)
cd frontend
npm run dev
```

---

## 📌 API Endpoints

### 🔐 Auth — `/api/auth`

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `POST` | `/signup` | Register with email or phone | ❌ |
| `POST` | `/send-otp` | Send OTP via email or SMS | ❌ |
| `POST` | `/verify-otp` | Verify OTP & receive JWT | ❌ |
| `GET` | `/logout` | Invalidate session | ✅ |

### 🧑‍💼 Portfolio — `/api/portfolio`

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| `POST` | `/create` | Submit portfolio details | ✅ |
| `GET` | `/:username` | Fetch generated portfolio | ❌ |
| `PUT` | `/update` | Update portfolio | ✅ |
| `DELETE` | `/delete` | Delete portfolio | ✅ |

### Example — Verify OTP

```bash
POST /api/auth/verify-otp
Content-Type: application/json

{
  "contact": "user@example.com",
  "otp": "49961"
}
```

```json
{
  "success": true,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...",
  "user": { "id": "64abc...", "email": "user@example.com" }
}
```

---

## 🌐 Portfolio Fields

```json
{
  "portfolioName": "My Portfolio",
  "personalInfo": {
    "name": "Ishan Bagra",
    "age": 20,
    "email": "ishanbagra18@gmail.com",
    "phone": "6377253179",
    "address": "A-116 Kardhani, Jaipur, Rajasthan"
  },
  "skills": [
    { "name": "JavaScript", "level": 89 },
    { "name": "Node.js",    "level": 75 },
    { "name": "React.js",   "level": 80 },
    { "name": "HTML",       "level": 90 },
    { "name": "CSS",        "level": 70 },
    { "name": "Angular",    "level": 65 }
  ],
  "education": [
    { "degree": "B.Tech", "institution": "IIIT Kota", "year": "2022 - Present" },
    { "degree": "College", "institution": "iiitkota",  "year": "2020 - 2022"   },
    { "degree": "School",  "institution": "St Teresa", "year": "2008 - 2020"   }
  ],
  "projects": [
    { "title": "Skylink",       "description": "Real-time in-flight communication system", "githubUrl": "..." },
    { "title": "Love-Advisor",  "description": "AI chatbot to resolve interpersonal conflicts", "githubUrl": "..." },
    { "title": "Dicegame",      "description": "A predictable dice game for timepass", "githubUrl": "..." }
  ],
  "competitiveProgramming": {
    "leetcode":  { "profile": "https://leetcode.com/u/ishanbagra/",       "rating": 1518 },
    "codechef":  { "profile": "https://www.codechef.com/START141D",       "rating": 1489 }
  },
  "contact": {
    "github": "https://github.com/...",
    "linkedin": "https://linkedin.com/in/...",
    "instagram": "https://instagram.com/...",
    "email": "ishanbagra18@gmail.com"
  }
}
```

---

## 🤝 Contributing

```bash
# 1. Fork this repo
# 2. Create your feature branch
git checkout -b feature/your-feature

# 3. Commit (Conventional Commits style)
git commit -m "feat: add your feature"

# 4. Push & open a Pull Request
git push origin feature/your-feature
```

---

## 📄 License

Licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

---

<div align="center">

Built with ❤️ by [Ishan Bagra](https://github.com/yourusername)

⭐ **Star this repo if you found it helpful!** ⭐

</div>
