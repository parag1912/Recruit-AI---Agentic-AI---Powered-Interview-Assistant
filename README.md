# 💼 Recruit-AI: Agentic AI-Powered Interview Assistant

---

## 📑 Table of Contents

1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Architecture & Flow Diagram](#architecture--flow-diagram)
4. [Features](#features)
5. [Tech Stack](#tech-stack)
6. [Project Structure](#project-structure)
7. [Setup & Installation](#setup--installation)
8. [Configuration Guide](#configuration-guide)
9. [Phase-Wise Roadmap](#phase-wise-roadmap)
10. [Development Workflow](#development-workflow)
11. [Contributing](#contributing)
12. [License](#license)

---

## 📖 Introduction

**Recruit-AI** is a full-stack, AI-powered mock interview platform designed to simulate realistic technical and behavioral interviews. Built with cutting-edge technologies like **Gemini AI**, **Next.js**, and **Clerk**, it offers interactive, real-time feedback tailored to user input—helping developers prepare more confidently for real-world interviews.

---

## 🌟 Project Overview

Recruit-AI provides users with an end-to-end interview simulation experience:
- Customized questions based on user-selected domains.
- Real-time AI-generated feedback to improve answers.
- Persistent user history and authentication for a personal journey.

Designed to be modular and extendable, Recruit-AI supports scalable user interactions and intelligent feedback loops.

---

## 🧠 Architecture & Flow Diagram

### 🔁 Flow Breakdown

1. **User Authentication**: Handled securely by Clerk.
2. **Interview Session Start**: User selects preferences (e.g., role, topic).
3. **AI-Generated Questions**: Sent to Gemini AI via API routes.
4. **User Answers**: Input stored and sent to AI for evaluation.
5. **Feedback Loop**: Gemini AI returns structured feedback.
6. **Result Storage**: Interview session stored via Drizzle ORM.

---

## ✨ Features

- 🤖 **Agentic Interview Simulation** – Tailored questions based on role, level, and topic.
- 🔐 **Clerk Auth Integration** – Secure user registration, login, and sessions.
- 🧠 **Gemini AI Feedback Engine** – Real-time analysis and tips on user answers.
- 📊 **User Dashboard** – Track progress across sessions and question types.
- 🔄 **Session Persistence** – Store and revisit past interviews.
- 📱 **Responsive UI** – Modern, mobile-friendly design.

---

## 🧰 Tech Stack

| Layer           | Tech                  |
|----------------|------------------------|
| Frontend       | Next.js 14, React, Tailwind CSS |
| Backend/API    | Next.js API Routes     |
| Auth           | Clerk.dev              |
| AI Engine      | Gemini AI (Google API) |
| ORM / Database | Drizzle ORM + PostgreSQL |
| State Mgmt     | React Hooks & Context  |

---

## 📁 Project Structure

```bash
ai-mock-interview/
├── app/                 # Next.js App Router
│   ├── interview/       # Interview logic & pages
│   ├── dashboard/       # User history and stats
│   └── api/             # Serverless API Routes
├── lib/                 # AI services, DB clients, utils
├── components/          # Reusable UI components
├── styles/              # Global Tailwind setup
├── drizzle/             # ORM schema & DB logic
├── public/              # Static assets
├── .env.example         # Environment configs
├── package.json         # NPM metadata
└── README.md
```

---

## 🛠️ Setup & Installation

### 🧾 Prerequisites
- Node.js 18+
- PostgreSQL instance (local/cloud)
- Gemini AI API Key
- Clerk account

### 🚀 Installation Steps

```bash
git clone https://github.com/amanbind898/ai-mock-interview.git
cd ai-mock-interview
npm install
cp .env.example .env
```

### 🧪 Development
```bash
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000) to test it locally.

---

## ⚙️ Configuration Guide

### Required .env Variables
| Key                     | Description                        |
|-------------------------|------------------------------------|
| CLERK_API_KEY           | Clerk API Key                      |
| NEXT_PUBLIC_CLERK_*     | Clerk Frontend Configs             |
| GEMINI_API_KEY          | Google Gemini AI Key               |
| DATABASE_URL            | PostgreSQL connection string       |

### Environment Tips
- You can use tools like **Railway**, **Neon**, or **Supabase** for PostgreSQL hosting.
- For Clerk setup, visit [Clerk Docs](https://clerk.dev/docs).

---

## 🗺️ Phase-Wise Roadmap

### ✅ Phase 1: MVP Complete
- Basic question generation (technical + behavioral)
- Real-time AI feedback
- User authentication & history

### 🚀 Phase 2: Feature Expansion
- Role-specific interview sets (Frontend, Backend, Data Science)
- Voice-based Q&A with Web Speech API
- Resume-based question parsing

### 🔮 Phase 3: Intelligence + Analytics
- Adaptive feedback based on past answers
- Strength/Weakness heatmaps
- Admin dashboard for managing question templates

---

## 🧪 Development Workflow

1. Fork & clone the repository
2. Create a feature branch:
```bash
git checkout -b feature/your-feature-name
```
3. Make changes and commit:
```bash
git commit -m "feat: add X"
```
4. Push and submit a PR

---

## 🤝 Contributing

We love contributors! Open issues, suggest features, and create PRs. Just follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).

---

## 📄 License

Licensed under [MIT License](LICENSE)

---

<div align="center">
  If this project helps you, please consider ⭐️ starring it!
</div>

