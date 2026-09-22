# Career-OS
CareerOS is a phone-first AI interview readiness platform that analyzes resumes and job descriptions, identifies personalized skill gaps, and conducts adaptive video interviews. AI turns each response into targeted follow-up questions, insights, and a focused practice plan—helping candidates prepare smarter for real interviews.
# 🚀 CareerOS

### Know your gaps. Practice smarter. Walk into the interview ready.

**CareerOS** is a phone-first AI-powered interview readiness platform designed to help students and job seekers prepare for real interviews through one personalized workflow.

Unlike traditional mock-interview platforms that rely on fixed question banks and generic scores, CareerOS analyzes the candidate's **resume, target Job Description (JD), and interview responses** to create an adaptive preparation experience.

---

## 🎯 Why CareerOS?

Interview preparation is often scattered across multiple tools:

* Resume analyzers
* Job description websites
* Generic interview question banks
* Mock interview platforms
* Communication practice tools
* Notes and preparation plans

CareerOS brings these steps together into **one personalized workflow**.

> **Your weaknesses determine what you practice next.**

---

# ✨ Key Features

## 📱 Phone-First Experience

CareerOS is designed around the smartphone as the **primary device**, rather than treating mobile as a smaller version of a desktop website.

Candidates can:

* Scan their resume using the phone camera
* Record interview answers
* Use their microphone and camera
* Practice interviews anywhere
* Receive immediate feedback

The laptop is used for deeper analysis, editing, and reviewing preparation.

---

## 📄 Resume Scanning & Analysis

Candidates can scan their resume using the phone camera or upload a PDF/DOCX from a laptop.

CareerOS extracts information such as:

* Skills
* Education
* Projects
* Work experience
* Achievements
* Technical knowledge
* Resume claims

The extracted information becomes the foundation for personalized interview preparation.

---

## 🎯 Job Description Analysis

Users provide the target Job Description.

CareerOS compares the candidate's resume with the requirements of the target role and identifies:

* Strengths
* Skill gaps
* Missing areas
* Resume risks
* Preparation priorities

This helps candidates understand **what they should focus on before the interview**.

---

# 🎙️ Adaptive AI Interview

The core experience of CareerOS is an interactive AI-powered interview.

Before starting, candidates can enable:

* 🎥 Camera
* 🎤 Microphone

The AI interviewer conducts a natural interview using synthetic speech, with support for different voice options.

Questions are generated based on:

* Candidate's resume
* Target role
* Job requirements
* Previous answers
* Detected weaknesses

---

## 🧠 The Adaptive Interview Loop

CareerOS does not simply ask a predefined list of questions.

Instead:

```text
Candidate Answer
       ↓
AI analyzes response
       ↓
Weakness detected
       ↓
Follow-up question generated
       ↓
Candidate answers again
       ↓
New weakness detected
       ↓
Next targeted question
```

### Example

A candidate explains a software architecture but does not discuss scalability.

CareerOS can identify:

> Missing discussion of scalability and trade-offs.

The next question can then explore:

> How would you scale this architecture if the number of users increased significantly?

This creates a **dynamic conversation instead of a scripted questionnaire**.

---

# 📊 Interview Analysis

After each response, CareerOS evaluates relevant dimensions such as:

* **Relevance**
* **Clarity**
* **Depth**
* **Structure**
* **Specificity**

Where supported, the system can also analyze delivery signals such as:

* Speaking pace
* Filler words
* Pauses
* Speech patterns

The purpose is to help candidates identify **specific areas for improvement**, rather than giving them a generic score.

---

# 📝 Resume Improvement

Interview weaknesses can also reveal problems in the candidate's resume.

CareerOS connects interview insights back to resume content and can provide concrete rewrite suggestions.

For example:

```text
Resume Claim
     ↓
Interview Follow-up
     ↓
Weakness Detected
     ↓
Resume Improvement Suggestion
```

This creates a feedback loop between **resume preparation and interview preparation**.

---

# 📅 Personalized Practice Plan

After the interview, CareerOS converts detected weaknesses into a focused practice plan.

The plan can include:

* What to practice
* Why it matters
* Suggested duration
* Specific objective
* Practice status

Instead of telling users to "practice more," CareerOS focuses their preparation on the weaknesses actually detected during their session.

---

# 📤 Shareable Readiness Snapshot

Candidates can generate a shareable snapshot containing:

* Readiness insights
* Key strengths
* Identified gaps
* Interview insights
* Resume improvement suggestions
* Practice plan

The snapshot can be used for:

* Personal review
* Mentor feedback
* Career guidance
* Interview preparation

Readiness indicators are intended as **preparation guidance**, not predictions of hiring outcomes.

---

# 💻📱 Phone → Laptop Workflow

CareerOS creates a natural workflow between devices.

### 📱 Phone

The phone is optimized for:

* Resume scanning
* Voice interaction
* Video interviews
* Camera capture
* Quick feedback
* Practice

### 💻 Laptop

The laptop is optimized for:

* Detailed analysis
* Reviewing insights
* Editing resume suggestions
* Reviewing practice plans
* Generating shareable snapshots

```text
        📱 PHONE
           │
   Scan → Speak → Interview
           │
           ↓
     AI Processing
           │
           ↓
        💻 LAPTOP
           │
   Review → Edit → Export
```

---

# 🏗️ Product Architecture

```text
┌──────────────────────────────────────────┐
│                CareerOS                  │
├──────────────────────────────────────────┤
│                                          │
│  📱 Phone Experience                     │
│  ├── Resume Camera                       │
│  ├── Microphone                          │
│  ├── Camera                              │
│  ├── Voice Interview                     │
│  └── Practice Feedback                   │
│                                          │
│  🧠 AI Layer                             │
│  ├── Resume Analysis                     │
│  ├── JD Analysis                         │
│  ├── Gap Detection                       │
│  ├── Question Generation                 │
│  └── Answer Analysis                     │
│                                          │
│  💻 Laptop Experience                    │
│  ├── Detailed Review                     │
│  ├── Resume Improvements                 │
│  ├── Practice Plan                       │
│  └── Snapshot Generation                 │
│                                          │
└──────────────────────────────────────────┘
```

---

# 🛠️ Tech Stack

### Frontend

* **Next.js**
* **TypeScript**
* **Tailwind CSS**
* **shadcn/ui**
* **Lucide Icons**

### State & Validation

* **Zustand**
* **React Hook Form**
* **Zod**

### Backend

* **Next.js Route Handlers**

### Database

* **Supabase PostgreSQL**

### Storage

* **Supabase Storage**

### AI

* LLM API
* Structured AI service layer

### Resume Parsing

* **PDF.js**
* **Mammoth**

### Voice

* **MediaRecorder API**
* **Web Audio API**

### Camera

* **getUserMedia**
* **MediaRecorder**

### On-Device Vision

* **MediaPipe**, where feasible

### Deployment

* **Vercel**
* **Supabase**

---

# 🗂️ Project Structure

```text
careeros/
│
├── app/
│   ├── page.tsx
│   ├── setup/
│   ├── analysis/
│   ├── interview/
│   ├── insights/
│   ├── practice/
│   └── snapshot/
│
├── components/
│   ├── ui/
│   ├── interview/
│   ├── resume/
│   ├── insights/
│   └── practice/
│
├── lib/
│   ├── ai/
│   │   ├── analyzeResume.ts
│   │   ├── analyzeJobDescription.ts
│   │   ├── detectGaps.ts
│   │   ├── generateQuestion.ts
│   │   └── analyzeAnswer.ts
│   │
│   ├── device/
│   │   ├── speech.ts
│   │   ├── audioAnalysis.ts
│   │   ├── camera.ts
│   │   └── eyeContact.ts
│   │
│   ├── parsers/
│   │   ├── resumePdf.ts
│   │   └── resumeDocx.ts
│   │
│   └── office-kit/
│       ├── syncSession.ts
│       └── generateSnapshot.ts
│
├── public/
│
├── supabase/
│
├── README.md
├── package.json
└── .env.example
```

---

# 🔄 Core User Journey

```text
Landing
   ↓
Resume + Job Description
   ↓
AI Analysis
   ↓
Readiness Report
   ↓
Adaptive Interview
   ↓
Interview Insights
   ↓
Personalized Practice Plan
   ↓
Shareable Snapshot
```

---

# 🔐 Privacy

Privacy is a core part of CareerOS.

The platform is designed around:

* Opt-in camera access
* Opt-in microphone access
* On-device voice/video processing where supported
* Clear data-handling communication
* User-controlled interview sessions

CareerOS does **not** attempt to predict whether a candidate will be hired.

Readiness indicators are designed to provide **preparation guidance**.

---

# ⚡ Getting Started

## 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/careeros.git
cd careeros
```

## 2. Install dependencies

```bash
npm install
```

## 3. Configure environment variables

Create a `.env.local` file:

```env
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
SUPABASE_SERVICE_ROLE_KEY=

AI_API_KEY=

NEXT_PUBLIC_APP_URL=
```

Add the appropriate values for your development environment.

## 4. Start the development server

```bash
npm run dev
```

Open:

```text
http://localhost:3000
```

---

# 🧪 Development

Run the development server:

```bash
npm run dev
```

Build the application:

```bash
npm run build
```

Start the production build:

```bash
npm start
```

Run linting:

```bash
npm run lint
```

---

# 🎨 Design Philosophy

CareerOS follows a **phone-first, action-oriented interface**.

The design focuses on:

* Clear next actions
* Minimal cognitive load
* Evidence-based insights
* Progressive disclosure
* Voice-first interaction
* Strong visual hierarchy
* Privacy visibility
* Seamless phone-to-laptop transitions

The interface takes inspiration from modern AI workspace products while adapting the experience specifically for interview preparation.

---

# 🏆 Hackathon Focus

CareerOS was designed around the **iQOO Hackathon's phone-first concept**.

The project focuses on:

| Area                  | CareerOS Approach                              |
| --------------------- | ---------------------------------------------- |
| Product Quality       | Complete interview preparation journey         |
| AI Innovation         | Weakness-driven adaptive questioning           |
| Phone Usage           | Camera, microphone and video-first interaction |
| Technical Depth       | AI + voice + camera + resume parsing           |
| Phone–Laptop Workflow | Practice on phone, deeper review on laptop     |
| User Impact           | Personalized interview preparation             |

---

# 💡 Core Innovation

Traditional mock interview:

```text
Question 1
   ↓
Question 2
   ↓
Question 3
   ↓
Question 4
```

CareerOS:

```text
Question
   ↓
Answer
   ↓
Analyze
   ↓
Find Weakness
   ↓
Generate Targeted Question
   ↓
Answer
   ↓
Analyze Again
   ↓
Continue
```

The interview therefore evolves based on the candidate's actual performance.

---

# 🚧 Current Scope

### Included

* Phone-first interview workflow
* Resume analysis
* Job description comparison
* Personalized gap detection
* Adaptive interview loop
* Voice interaction
* Optional camera interaction
* Interview insights
* Resume rewrite suggestions
* Personalized practice plan
* Shareable readiness snapshot
* Phone-to-laptop workflow

### Out of Scope

* Hiring probability prediction
* Persistent career memory across multiple sessions
* Advanced body-language scoring
* Full multilingual support
* Complex account systems unless required
* Static bottom navigation as the primary interaction model

---

# 🔮 Future Possibilities

Potential future improvements include:

* More advanced on-device speech analysis
* Expanded role-specific interview models
* More detailed interview simulations
* Mentor collaboration
* Career-session history
* Additional language support
* Deeper resume optimization
* Industry-specific preparation paths

---

# 👥 Team

Built for the **iQOO Hackathon 2026**.

**Project:** CareerOS
**Category:** AI × Career Technology × Interview Preparation
**Platform:** Phone-first Web Application

---

# 📜 License

This project is developed as a hackathon project.

Add your preferred open-source license here if the project will be publicly distributed.

---

## 🚀 CareerOS

**Know your gaps. Practice smarter. Walk into the interview ready.**

