#  SkillMap — AI Skill Assessment & Personalized Learning Agent

SkillMap is an AI-powered web application that evaluates a candidate’s real technical skills by analyzing their **resume** and a **job description**, then conducts a **conversational assessment** and generates a **structured learning roadmap**.

Unlike traditional resume screening, SkillMap focuses on **actual skill depth**, not just keywords.

---

##  Project Objective

A resume only shows what a candidate claims to know.  
This project solves that gap by:

- Assessing real understanding through AI-driven questions
- Identifying skill gaps
- Predicting interview probability
- Generating a personalized 16-week learning plan

---

##  Key Features

###  AI-Based Skill Assessment
- Extracts required skills from Job Description
- Asks **real-world, scenario-based questions**
- Evaluates answers conversationally

###  Smart Skill Analysis
- Classifies skills as:
  - Strong
  - Partial
  - Gap
- Assigns scores for each skill

###  ATS Match Score
- Calculates resume alignment with job description
- Shows:
  - Matching skills
  - Missing skills

###  Interview Probability Prediction
- Predicts chances of getting shortlisted
- Provides reasoning behind the score

###  Readiness Meter
- Shows:
  - Current readiness
  - Expected readiness after improvement

###  16-Week Learning Roadmap
- Weekly structured plan
- Task-based learning approach
- Focus on practical skills

---

##  Tech Stack

### Frontend
- HTML5
- CSS3 (Custom UI Design)
- Vanilla JavaScript

### AI Integration
- Claude (Anthropic API)

### Other Concepts
- File Upload Handling (PDF, DOCX, TXT)
- Base64 Encoding for documents
- Conversational AI flow
- Dynamic DOM rendering

---

##  How It Works

1. User uploads Resume or pastes text
2. User enters Job Description
3. AI:
   - Extracts required skills
   - Starts conversational interview
4. User answers questions
5. AI generates final report:
   - Skill scores
   - ATS score
   - Interview probability
   - Learning roadmap

---

##  Note:

> ⚠️ This project uses the Anthropic API directly from the browser.

- It is designed to run within environments like **Claude.ai**, where API access is already handled internally.
- In such environments, **no API key is required** from the user side.
- If you run this project outside Claude.ai (e.g., locally or via Netlify), you will need to:
  - Provide your own Anthropic API key
  - Modify the request headers accordingly

👉 For production use, it is strongly recommended to:
- Use a backend (Node.js / Flask) to securely handle API calls
- Avoid exposing API keys in frontend code
