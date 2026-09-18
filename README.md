# AI-Powered Interview Preparation & Career Assistant

An AI-powered full-stack web application that helps candidates prepare for technical and behavioral interviews by analyzing a job description, candidate profile, and resume.

The application uses Google's Gemini API to generate personalized interview questions, identify skill gaps, and create a customized interview preparation roadmap.

---

## 🚀 Features

- 📄 Job Description Analysis
- 👤 Candidate Profile Analysis
- 📑 Resume Processing
- 🤖 AI-powered Interview Strategy
- 💻 Technical Interview Questions
- 🧠 Behavioral Interview Questions
- 📊 Skill Gap Analysis
- 🗺️ Personalized Preparation Roadmap
- 🔐 JWT-based Authentication
- 💾 MongoDB-based Report Storage
- 📄 PDF Report Generation
- ⚡ React-based User Interface

---

## 🛠️ Tech Stack

### Frontend

- React.js
- Vite
- Axios
- JavaScript
- HTML
- CSS

### Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication

### Generative AI

- Google Gemini API
- Generative AI

### Other Technologies

- PDF Processing
- Puppeteer

---

## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │       User          │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   React Frontend    │
                    │      + Vite         │
                    └──────────┬──────────┘
                               │
                         HTTP / Axios
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Node.js + Express │
                    │      Backend        │
                    └──────────┬──────────┘
                               │
                ┌──────────────┼──────────────┐
                │              │              │
                ▼              ▼              ▼
          ┌──────────┐   ┌──────────┐   ┌──────────────┐
          │   JWT    │   │ MongoDB  │   │ Gemini API   │
          │   Auth   │   │ Database │   │  Generative  │
          └──────────┘   └──────────┘   │      AI      │
                                        └──────────────┘
                                               │
                                               ▼
                                  Personalized Interview
                                       Preparation

# Application Workflow

User
  │
  ▼
Enter Job Description
  │
  ▼
Enter Candidate Information
  │
  ▼
Upload Resume
  │
  ▼
React Frontend
  │
  ▼
Express Backend
  │
  ▼
Process Candidate Data
  │
  ▼
Google Gemini API
  │
  ▼
Generate Interview Strategy
  │
  ├── Technical Questions
  ├── Behavioral Questions
  ├── Skill Gap Analysis
  └── Preparation Roadmap
  │
  ▼
Store Report in MongoDB
  │
  ▼
Display Report in React
