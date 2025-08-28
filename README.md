# Jobly AI — MERN Job Posting & Applications (Clerk + OpenAI)

> Admins post jobs. Candidates apply with answers.  
> A custom OpenAI model scores answers as **Bad / Moderate / Good** based on the job role and responses.  
> Built with **MERN** (Backend in **TypeScript**, Frontend in **JavaScript**) and **Clerk** for auth.

---

## ✨ Features

- **Admin**
  - Create/Read/Update/Delete job posts (title, type, location, description, questions)
  - View all applications per job
  - See AI rating for each candidate’s answers (**Bad / Moderate / Good**)

- **Candidate**
  - Browse jobs
  - Submit application + answers to job-specific questions
  - Get feedback/rating (via the custom OpenAI model)

- **Platform**
  - Auth & sessions with **Clerk**
  - Backend: **Node.js + Express + TypeScript + Mongoose**
  - Frontend: **React (Vite) + JS**
  - OpenAI custom model for scoring answers

---

## 🏗 Tech Stack

- **Frontend:** React (Vite), JavaScript, Axios, Shadcn UI/Lucide (optional)
- **Backend:** Node.js, Express, TypeScript, Mongoose/MongoDB
- **Auth:** Clerk
- **AI:** OpenAI (custom model / fine-tuned logic)
- **Tooling:** dotenv, Zod (validation), CORS

---

## 📁 Monorepo Structure

job-app/
├─ backend/ # Express + TS (Clerk, OpenAI, MongoDB)
├─ frontend/ # React + Vite (JS)
├─ .gitignore
├─ README.md
└─ LICENSE


---

## ⚙️ Environment Setup

1. **Clone**

   ```bash
   git clone https://github.com/<your-username>/job-app.git
   cd job-app

2. **Backend env**
   cp backend/.env.example backend/.env
# fill MONGODB_URI, CLERK keys, OPENAI_API_KEY, etc.

3. **Frontend env**
   cp frontend/.env.example frontend/.env
# set VITE_API_BASE_URL & VITE_CLERK_PUBLISHABLE_KEY
