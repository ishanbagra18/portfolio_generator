<div align="center">

<img src="https://img.shields.io/badge/Portfolio-Generator-6C63FF?style=for-the-badge&logo=firefox&logoColor=white" alt="Portfolio Generator" height="50"/>

# 🚀 Portfolio Generator with OTP Authentication

**Transform your details into a stunning portfolio — in minutes.**

[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Nodemailer](https://img.shields.io/badge/Nodemailer-0A7BBB?style=for-the-badge&logo=gmail&logoColor=white)](https://nodemailer.com/)
[![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=twilio&logoColor=white)](https://www.twilio.com/)

<br/>

![GitHub stars](https://img.shields.io/github/stars/yourusername/portfolio-generator?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/portfolio-generator?style=social)
![GitHub issues](https://img.shields.io/github/issues/yourusername/portfolio-generator?color=red)
![License](https://img.shields.io/github/license/yourusername/portfolio-generator?color=blue)

<br/>

> 🔐 **Secure** · ⚡ **Fast** · 🎨 **Beautiful** · 📱 **Responsive**

</div>

---

## 📋 Table of Contents

- [✨ Overview](#-overview)
- [🔐 Authentication Flow](#-authentication-flow)
- [🎯 Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ Installation](#️-installation)
- [🔧 Configuration](#-configuration)
- [🚀 Running the App](#-running-the-app)
- [📌 API Endpoints](#-api-endpoints)
- [🌐 Portfolio Fields](#-portfolio-fields)
- [📸 Screenshots](#-screenshots)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Overview

**Portfolio Generator** is a full-stack web application that allows users to register, authenticate via OTP (email or SMS), fill in their professional details, and instantly receive a beautifully generated portfolio website — all without writing a single line of code.

```
User Signs Up → Receives OTP → Logs In → Fills Profile → Gets Portfolio 🎉
```

---

## 🔐 Authentication Flow

```
┌─────────────┐       ┌──────────────────┐       ┌──────────────────┐
│   Sign Up   │──────▶│  OTP Delivered   │──────▶│    Dashboard     │
│ Email/Phone │       │  📧 Email or     │       │  Build Portfolio │
└─────────────┘       │  📱 SMS (Twilio) │       └──────────────────┘
                       └──────────────────┘
```

| Method | Provider | Delivery Time |
|--------|----------|--------------|
| 📧 Email OTP | Nodemailer (SMTP/Gmail) | < 30 seconds |
| 📱 SMS OTP | Twilio | < 10 seconds |

- OTPs are **time-limited** (expire in 5–10 minutes)
- Each OTP is **single-use** — invalidated after verification
- No passwords stored — completely **passwordless auth**

---

## 🎯 Features

### 🔑 Authentication
- ✅ Sign up with **email** or **phone number**
- ✅ Login via **OTP** — no password needed
- ✅ OTP delivery via **Nodemailer** (email) and **Twilio** (SMS)
- ✅ OTP expiry and rate limiting
- ✅ Secure session management with **JWT**

### 🧑‍💼 Portfolio Builder
- ✅ Collects comprehensive professional data
- ✅ Automatically generates a **personalized portfolio website**
- ✅ Fully responsive and mobile-friendly output
- ✅ Multiple portfolio **themes/templates**
- ✅ Shareable public portfolio URL

### 🛡️ Security
- ✅ OTP hashed before storing in DB
- ✅ JWT-based protected routes
- ✅ Input validation and sanitization
- ✅ Rate limiting on OTP requests

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|-----------|---------|
| HTML5 / CSS3 | Markup & Styling |
| JavaScript (ES6+) | Client-side logic |
| *(React — optional)* | Component-based UI |

### Backend
| Technology | Purpose |
|-----------|---------|
| **Node.js** | Runtime environment |
| **Express.js** | Web framework & REST API |
| **JWT** | Secure session tokens |
| **bcrypt** | OTP hashing |

### OTP / Messaging
| Service | Purpose |
|--------|---------|
| **Nodemailer** | Email OTP delivery (SMTP/Gmail) |
| **Twilio** | SMS OTP delivery |

### Database
| Technology | Purpose |
|-----------|---------|
| **MongoDB** | User data & session storage |
| **Mongoose** | ODM for schema modeling |

---

## 📁 Project Structure

```
portfolio-generator/
│
├── 📂 backend/
│   ├── 📂 config/
│   │   ├── db.js              # MongoDB connection
│   │   └── nodemailer.js      # Email transport setup
│   │
│   ├── 📂 controllers/
│   │   ├── authController.js  # Signup, login, OTP logic
│   │   └── portfolioController.js
│   │
│   ├── 📂 middleware/
│   │   ├── authMiddleware.js  # JWT verification
│   │   └── rateLimiter.js     # OTP rate limiting
│   │
│   ├── 📂 models/
│   │   ├── User.js            # User schema
│   │   ├── OTP.js             # OTP schema
│   │   └── Portfolio.js       # Portfolio schema
│   │
│   ├── 📂 routes/
│   │   ├── authRoutes.js      # /api/auth/*
│   │   └── portfolioRoutes.js # /api/portfolio/*
│   │
│   ├── 📂 services/
│   │   ├── emailService.js    # Nodemailer OTP email
│   │   └── smsService.js      # Twilio OTP SMS
│   │
│   ├── .env                   # Environment variables
│   ├── server.js              # Entry point
│   └── package.json
│
├── 📂 frontend/
│   ├── 📂 public/
│   ├── 📂 src/
│   │   ├── index.html
│   │   ├── login.html
│   │   ├── signup.html
│   │   └── dashboard.html
│   └── 📂 assets/
│
└── README.md
```

---

## ⚙️ Installation

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) v16+
- [MongoDB](https://www.mongodb.com/) (local or Atlas)
- A [Twilio](https://www.twilio.com/) account *(for SMS OTP)*
- A Gmail or SMTP account *(for email OTP)*

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/portfolio-generator.git
cd portfolio-generator
```

### 2. Install Dependencies

```bash
# Backend
cd backend
npm install

# Frontend (if React-based)
cd ../frontend
npm install
```

---

## 🔧 Configuration

Create a `.env` file in the `/backend` directory:

```env
# ── Server ───────────────────────────────────────
PORT=5000
NODE_ENV=development

# ── Database ─────────────────────────────────────
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/portfolio_db

# ── JWT ──────────────────────────────────────────
JWT_SECRET=your_super_secret_jwt_key
JWT_EXPIRES_IN=7d

# ── OTP Settings ─────────────────────────────────
OTP_EXPIRY_MINUTES=10

# ── Nodemailer (Email OTP) ────────────────────────
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password        # Use Gmail App Password

# ── Twilio (SMS OTP) ─────────────────────────────
TWILIO_ACCOUNT_SID=ACxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_PHONE_NUMBER=+1234567890
```

> ⚠️ **Never commit your `.env` file.** Add it to `.gitignore`.

---

## 🚀 Running the App

### Development Mode

```bash
# Start backend
cd backend
npm run dev        # Uses nodemon for hot-reload

# Start frontend (in a separate terminal)
cd frontend
npm start
```

### Production Mode

```bash
cd backend
npm start
```

The app will run at: **`http://localhost:5000`**

---

## 📌 API Endpoints

### 🔐 Auth Routes — `/api/auth`

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| `POST` | `/signup` | Register with email or phone | ❌ |
| `POST` | `/send-otp` | Send OTP to email or phone | ❌ |
| `POST` | `/verify-otp` | Verify OTP & receive JWT | ❌ |
| `GET` | `/logout` | Invalidate current session | ✅ |

### 🧑‍💼 Portfolio Routes — `/api/portfolio`

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| `POST` | `/create` | Submit portfolio details | ✅ |
| `GET` | `/:username` | Get public portfolio | ❌ |
| `PUT` | `/update` | Update portfolio details | ✅ |
| `DELETE` | `/delete` | Delete portfolio | ✅ |

### Example — Send OTP

```bash
POST /api/auth/send-otp
Content-Type: application/json

{
  "contact": "user@example.com",   # or phone: "+919876543210"
  "method": "email"                # or "sms"
}
```

**Response:**
```json
{
  "success": true,
  "message": "OTP sent successfully",
  "expiresIn": "10 minutes"
}
```

---

## 🌐 Portfolio Fields

When building a portfolio, the following data is collected:

```json
{
  "personalInfo": {
    "fullName": "Jane Doe",
    "title": "Full Stack Developer",
    "bio": "Passionate developer with 3 years of experience...",
    "avatar": "https://link-to-photo.com/photo.jpg",
    "location": "Mumbai, India"
  },
  "contact": {
    "email": "jane@example.com",
    "phone": "+91-9876543210",
    "linkedin": "https://linkedin.com/in/janedoe",
    "github": "https://github.com/janedoe",
    "website": "https://janedoe.dev"
  },
  "skills": ["JavaScript", "Node.js", "React", "MongoDB", "Docker"],
  "projects": [
    {
      "title": "Portfolio Generator",
      "description": "An OTP-based portfolio builder...",
      "techStack": ["Node.js", "Express", "MongoDB"],
      "liveUrl": "https://demo.com",
      "githubUrl": "https://github.com/user/repo"
    }
  ],
  "education": [
    {
      "degree": "B.Tech in Computer Science",
      "institution": "IIT Bombay",
      "year": "2020–2024",
      "grade": "8.9 CGPA"
    }
  ],
  "experience": [
    {
      "company": "TechCorp",
      "role": "Backend Developer",
      "duration": "June 2024 – Present",
      "description": "Built RESTful APIs serving 100k+ users..."
    }
  ],
  "achievements": ["Hackathon Winner 2023", "Open Source Contributor"],
  "languages": ["English", "Hindi", "Gujarati"],
  "certifications": [
    {
      "name": "AWS Certified Developer",
      "issuer": "Amazon",
      "year": "2023"
    }
  ]
}
```

---

## 📸 Screenshots

> 📷 *(Add your actual screenshots by replacing the placeholders below)*

| Signup Page | OTP Verification | Portfolio Dashboard |
|:-----------:|:----------------:|:-------------------:|
| ![Signup](https://via.placeholder.com/300x200?text=Signup+Page) | ![OTP](https://via.placeholder.com/300x200?text=OTP+Verification) | ![Dashboard](https://via.placeholder.com/300x200?text=Dashboard) |

| Portfolio Builder | Generated Portfolio |
|:-----------------:|:-------------------:|
| ![Builder](https://via.placeholder.com/400x220?text=Portfolio+Builder) | ![Portfolio](https://via.placeholder.com/400x220?text=Generated+Portfolio) |

---

## 🤝 Contributing

Contributions are welcome and appreciated! 🙌

```bash
# 1. Fork the repository
# 2. Create your feature branch
git checkout -b feature/amazing-feature

# 3. Commit your changes
git commit -m "feat: add amazing feature"

# 4. Push to the branch
git push origin feature/amazing-feature

# 5. Open a Pull Request
```

Please follow the [Conventional Commits](https://www.conventionalcommits.org/) standard for commit messages.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

Made with ❤️ by [Your Name](https://github.com/yourusername)

⭐ **Star this repo if you found it helpful!** ⭐

</div>
