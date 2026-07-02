# 🚀 DeadlineCopilot

An AI-powered productivity companion that helps students and professionals stay ahead of deadlines instead of reacting to them.

Built by [Farzeen Fatima](https://github.com/FarzeenFatima55).

---

## 📖 Overview

Managing multiple assignments, projects, meetings, and deadlines is overwhelming. Traditional task managers only remind users after tasks are already planned.

**DeadlineCopilot** acts as an intelligent productivity companion that:

- Prioritizes deadlines automatically
- Uses AI to analyze and summarize tasks
- Captures work from images and documents
- Integrates directly with Google Calendar
- Keeps productivity features available even when external AI services are unavailable

---

## ✨ Features

### 🔐 Google Authentication
- Secure Firebase Authentication
- One-click Google Sign In
- Persistent user sessions

### 📅 Smart Deadline Management
- Create and organize deadlines
- Track upcoming work
- Priority-based task organization

### 🤖 AI Task Analysis
Powered by Google Gemini
- Task summarization
- Intelligent insights
- AI-generated recommendations
- Productivity assistance

### 📷 Capture Hub
Extract information from images, notes, and documents. AI converts captured information into actionable tasks.

### 📆 Google Calendar Integration
- Connect Google Calendar
- Sync events
- View upcoming schedule
- Stay organized across platforms

### ⚡ Modern Dashboard
- Responsive UI
- Clean, productivity-focused interface
- Fast performance using Next.js

---

## 🛠 Tech Stack

**Frontend**
- Next.js 16
- React 19
- TypeScript
- Tailwind CSS
- Framer Motion

**Backend / Services**
- Firebase Authentication
- Cloud Firestore
- Google Gemini API
- Google Calendar API

**Deployment**
- Google Cloud Run

---

## 🏗 Architecture

```
                User
                  │
                  ▼
         Next.js Frontend
                  │
      ┌───────────┼────────────┐
      ▼           ▼            ▼
 Firebase      Gemini AI   Google Calendar
 Authentication    API          API
      │
      ▼
 Cloud Firestore
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/FarzeenFatima55/DeadlineCopilot.git
cd DeadlineCopilot/frontend
```

### 2. Install dependencies

```bash
npm install --legacy-peer-deps
```

### 3. Set up environment variables

Create a `.env.local` file in the `frontend` folder:

```env
NEXT_PUBLIC_FIREBASE_API_KEY=YOUR_KEY
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=YOUR_DOMAIN
NEXT_PUBLIC_FIREBASE_PROJECT_ID=YOUR_PROJECT
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=YOUR_BUCKET
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=YOUR_SENDER_ID
NEXT_PUBLIC_FIREBASE_APP_ID=YOUR_APP_ID

GEMINI_API_KEY=YOUR_GEMINI_KEY

GOOGLE_CALENDAR_CLIENT_ID=YOUR_CLIENT_ID
GOOGLE_CALENDAR_CLIENT_SECRET=YOUR_SECRET
GOOGLE_CALENDAR_COOKIE_SECRET=YOUR_COOKIE_SECRET
```

### 4. Run locally

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📂 Project Structure

```
frontend/
│
├── app/            # Routes and pages (Next.js App Router)
├── components/     # Reusable UI components
├── hooks/          # Custom React hooks (auth, tasks, etc.)
├── lib/            # Firebase config, Gemini API calls, utilities
├── public/         # Static assets
├── src/            # Core source files
│
├── package.json
└── Dockerfile
```

---

## ☁ Deployment

Deployed on **Google Cloud Run**.

```bash
gcloud run deploy --source .
```

*Live demo link coming soon.*

---

## 🎯 Problem Statement

Students and professionals often struggle with:

- Multiple overlapping deadlines
- Missed assignments
- Poor task prioritization
- Fragmented productivity tools across platforms

**DeadlineCopilot** combines AI assistance, task management, and calendar integration into one unified productivity platform — built to help people stay ahead, not catch up.

---

## 🔮 Future Improvements

- [ ] AI-based deadline prediction
- [ ] Email integration
- [ ] Team collaboration features
- [ ] Smart notification system
- [ ] Mobile application
- [ ] Offline support
- [ ] AI-powered productivity analytics

---

## 👩‍💻 Author

**Farzeen Fatima**
Web Developer | AI Automation Engineer | CS Student @ Sukkur IBA University

- GitHub: [@FarzeenFatima55](https://github.com/FarzeenFatima55)

---

## 📄 License

This project is open for learning and personal use. Feel free to fork and build on it.
