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
```

---

## 🔄 Application Workflow

```text

User
  │
  ▼
Login / Register
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
Process Input Data
  │
  ▼
Google Gemini API
  │
  ├── Technical Questions
  ├── Behavioral Questions
  ├── Skill Gap Analysis
  ├── Interview Strategy
  └── Preparation Roadmap
  │
  ▼
Store Report in MongoDB
  │
  ▼
Display Report in React

```

---

## 🤖 Generative AI Integration

This project uses Generative AI through the Google Gemini API.

The backend sends relevant candidate information and job requirements to Gemini.

```text
Job Description
       +
Candidate Profile
       +
Resume Information
       │
       ▼
   AI Prompt
       │
       ▼
 Google Gemini
       │
       ▼
Generated Interview Content

```

---

## 🔌 API Communication

The React frontend communicates with the Node.js backend using REST APIs.

```text
React Frontend
      │
      │ Axios / HTTP Request
      ▼
Express Routes
      │
      ▼
Controllers
      │
      ▼
Services
      │
      ▼
Gemini API / MongoDB
      │
      ▼
Backend Response
      │
      ▼
React Frontend

```

---

## 🔐 Authentication

The application uses JWT (JSON Web Token) based authentication.

```text
User
 │
 ▼
Login / Register
 │
 ▼
Backend
 │
 ▼
Validate Credentials
 │
 ▼
Generate JWT
 │
 ▼
Frontend
 │
 ▼
Authenticated API Requests

```

---

## 💾 Database

The application uses MongoDB as the database.

Mongoose is used as the ODM layer for interacting with MongoDB.

The database can store:

- User information
- Interview reports
- Generated interview content
- Candidate information

```text
Node.js Backend
      │
      ▼
   Mongoose
      │
      ▼
    MongoDB
```

---

## 📄 Resume Processing

The application supports resume upload and processing.

```text
Resume File
     │
     ▼
Backend Upload
     │
     ▼
PDF Processing
     │
     ▼
Extract Resume Information
     │
     ▼
Combine With Candidate Data
     │
     ▼
Gemini API
```

---

# 🖥️ Screenshots

## Home Page

![Login Page](https://github.com/karanAI01/ai-interview-preparation/blob/main/screenshots/Login%20.png)

## Interview Strategy

![Interview Strategy](https://github.com/karanAI01/ai-interview-preparation/blob/main/screenshots/interview%20plan%20.png)

## Technical Questions

![Technical Questions]()

## Skill Gap Analysis

![Skill Gap Analysis]()
