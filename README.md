# Synapse Classroom

> A unified platform bridging personal understanding with dynamic peer interaction.

## The Problem Statement
Students often take unstructured, context-dependent notes during fast-paced lectures, which become difficult to understand over time. This leads to inefficient revision, where learners spend more time re-learning than reinforcing concepts. 

At the same time, peer learning remains underutilized due to social hesitation, lack of suitable partners, and the absence of structured collaboration systems. The disconnect between individual note-taking and collaborative learning results in poor knowledge retention, reduced engagement, and increased academic stress. 

Currently, a unified approach that bridges personal understanding with peer interaction is missing.

---

## Our Solution
Synapse Classroom completely rethinks the educational experience by combining AI-driven personal study tools with engaging, gamified social peer learning. We turn chaotic lecture notes into structured pathways and transform intimidating group study sessions into stress-free "Boss Raids."

## Key Features & User Workflows

### Part 1: Teacher Features

#### 1. Automated Curriculum Hub & Quiz Generation
**Primary Benefit:** Bridges the overall learning ecosystem

**User Workflow:**
1. A teacher creates a Classroom and uploads their curriculum materials (PDFs, presentations, documents) to the portal.
2. The teacher clicks a single button to auto-generate a structured, adaptive quiz based directly on the uploaded material text.
3. The quiz is automatically distributed to the dashboards of all remotely enrolled students.

**Reason for adding:** While the platform heavily focuses on peer-to-peer and self-driven learning, keeping the teacher in the loop ensures the collaboration actually stays tethered to the real-world curriculum without creating extra manual work for the instructor.

#### 2. Real-Time Analytics Dashboard
**Primary Benefit:** Streamlined, automated evaluation

**User Workflow:**
1. Students complete the assigned AI-generated quizzes in their own time, earning XP on their gamified dashboard.
2. The teacher opens their Analytics Dashboard, which automatically aggregates the student scores in real-time.
3. The dashboard categorizes performers (e.g., Weak, Average, Topper) and provides a macro-level view of classroom health without any manual grading.

**Reason for adding:** Eliminates grading overhead and allows instructors to quickly identify systemic knowledge gaps or underperforming students before major offline exams or standardized tests.

---

### Part 2: Student Features

#### 1. AI Notes Refiner & Mistake Corner
**Primary Benefit:** Enhances Efficient Revision

**User Workflow:**
1. A student uploads messy, rushed lecture notes or confusing class materials to their student portal.
2. The integrated AI instantly processes the text into clean summaries, structured topic tags, and generates interactive flashcards.
3. As the student studies the flashcards and takes automated quizzes, the system tracks their performance.
4. Any incorrect answers are securely logged in the "Mistake Corner," where a personalized AI Tutor explains the specific mathematical or conceptual error and offers targeted re-testing.

**Reason for adding:** This directly solves the issue of inefficient revision. Instead of spending hours deciphering fast-paced notes, learners immediately receive structured contexts, turning failures into personalized learning opportunities and shifting their time from re-learning to active reinforcement.

#### 2. Gamified Boss Raids (Multiplayer Quizzes)
**Primary Benefit:** Enhances Peer Collaboration

**User Workflow:**
1. A student navigates to the Classmates tab to view peers and seamlessly sends a friend request.
2. Once connected, a student challenges their friend to a private, 1v1 "Boss Battle."
3. A dynamic boss arena spawns. Both students independently answer quiz questions pulled directly from their actively enrolled subjects to deal continuous "damage" to the boss.
4. If their combined performance successfully defeats the boss, both players earn joint XP, strengthen their daily activity streak, and receive exclusive Raid Badges displayed permanently on their profile.

**Reason for adding:** This tackles the "underutilized peer learning" problem. By presenting peer collaboration as a low-pressure, familiar RPG-style game, we eliminate social hesitation. It provides an immediate, structured collaboration system that motivates peers to succeed together without requiring a teacher's oversight.

#### 3. Interactive Learning Dashboard
**Primary Benefit:** Enhances Revision Motivation and Long-term Engagement

**User Workflow:**
1. A student logs into their dashboard and sees an overview of their Total XP, Daily Streak, and earned Boss Raid Badges.
2. The Global Leaderboard displays the top students across all classrooms, visually tracking the most dedicated learners.
3. The student is motivated by the premium, intuitive UI to maintain their daily streak and interact with both the AI Tutor and their friends.

**Reason for adding:** To completely eliminate "reduced engagement." A visually stunning interface backed up by genuine gamified rewards builds positive reinforcement, making students want to interact with the platform and each other daily rather than viewing studying as a chore.

---

## Technology Stack
* **Frontend:** React, Vite (featuring a custom, responsive CSS Glassmorphism aesthetic)
* **Backend:** Python, Flask, Local SQLite (For robust data integrity and fast deployments)
* **AI Integrations:** Groq (llama3.1-8b)-complient LLM APIs powering the Tutor and Note Refiners
* **Authentication:** Firebase Auth

## How to Run Locally

### 1. Start the Backend
Navigate to the backend directory, install the Python requirements, and run the developer server:
```bash
cd synapse-backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python run.py
```

### 2. Start the Frontend
In a new terminal, navigate to the frontend directory, install the node modules, and start Vite:
```bash
cd synapse-frontend
npm install
npm run dev
```

Visit `http://localhost:5173` to experience Synapse Classroom.
