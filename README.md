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

## How It Works

1. User enters the job description.
2. User provides their profile information and resume.
3. Frontend sends the information to the backend.
4. Backend processes the data.
5. Google Gemini generates personalized interview content.
6. The generated report is stored in MongoDB.
7. The frontend displays the interview preparation report.

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
