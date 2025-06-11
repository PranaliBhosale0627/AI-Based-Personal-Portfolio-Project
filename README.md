# AI-Based-Personal-Portfolio-Project

An intelligent web application that automatically generates professional portfolios by analyzing resumes using AI. Ideal for students, professionals, and job seekers, this tool helps showcase skills, achievements, and projects in a dynamic and elegant format.

---

## 📚 Table of Contents

- [🔍 Project Overview](#-project-overview)
- [✨ Features](#-features)
- [🧰 Tech Stack](#-tech-stack)
- [🏗️ Architecture & Design](#-architecture--design)
- [📦 Installation Guide](#-installation-guide)
- [🚀 Usage Instructions](#-usage-instructions)
- [📁 Project Structure](#-project-structure)
- [📸 Screenshots](#-screenshots)
- [👨‍💻 Contributors](#-contributors)
- [📄 License](#-license)

---

## 🔍 Project Overview

This project aims to automate the process of building personal portfolios using AI. By simply uploading a resume, users can generate interactive, aesthetically pleasing portfolios with minimal manual input. The system integrates OpenAI’s language model to extract, summarize, and reformat information from resumes.

---

## ✨ Features

- 🔐 User Registration & Login
- 📄 Resume Upload (PDF format)
- 🧠 AI-powered data extraction (summaries, keywords, achievements)
- 🎨 Dynamic Portfolio Templates
- 👀 Live Preview of Portfolio
- 📥 Download final version in PDF/HTML format
- 🎛 Admin/Doctor/Patient role management (for demo/test scenarios)

---

## 🧰 Tech Stack

### 💻 Frontend:
- HTML5, CSS3
- JavaScript (Vanilla)
- Bootstrap
- Jinja2 Templating

### 🖥️ Backend:
- Python 3.x
- Flask
- Flask-Login (Authentication)
- Flask-SQLAlchemy (ORM)

### 🧠 AI & NLP:
- OpenAI GPT (via API)
- Resume Parser (PDF-to-Text)

### 🗄️ Database:
- SQLite (development)
- MySQL/PostgreSQL (production-ready)

---

## 🏗️ Architecture & Design

```plaintext
User
  │
  ├── Upload Resume
  │     ↓
Frontend (Form)
  │
  ├──→ Flask App (Backend)
         │
         ├──→ AI Engine (GPT/Parser)
         │     ↓
         ├──→ Portfolio Generator
         │     ↓
         └──→ Database (User Info, Portfolio, Resume)
  ↓
Preview/Download Portfolio (HTML/PDF)
