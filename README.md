# 📬 MailMind AI

### Turn messy emails into clear actions.

**MailMind AI** is an AI-powered email intelligence assistant that transforms unstructured emails into concise, actionable insights.

Instead of simply summarizing an email, MailMind answers:

> **What is this email about? How important is it? What do I need to do? When do I need to do it? Is it safe? And should I reply?**

---

## 🚀 Live Demo

🔗 **Demo:** `ADD_DEPLOYED_LINK_HERE`

🔗 **Repository:** `ADD_GITHUB_LINK_HERE`

---

## 🎯 Problem

Students and professionals receive dozens of emails every day.

Important information is often buried inside long messages, making it difficult to quickly identify:

* What actually matters
* Which emails require action
* Which tasks have deadlines
* Which messages are urgent
* Whether an email may be phishing
* How to respond appropriately

Manually processing every email takes time and can lead to missed deadlines and delayed responses.

---

## 💡 Solution

MailMind AI converts an unstructured email into structured, actionable intelligence.

### One email → one decision-ready output

📧 **Email**

↓

📝 Summary

🚦 Priority

🏷️ Category

✅ Tasks

⏰ Deadlines

🛡️ Security Analysis

💬 Reply Suggestion

---

## ✨ Core Features

### 📧 Smart Summarization

Creates a concise summary while preserving important context.

### 🚦 Priority Detection

Classifies emails as:

* 🔴 High
* 🟡 Medium
* 🟢 Low

Priority is determined using evidence such as urgency, deadlines, required action, consequences of delay, and context.

### 🏷️ Email Categorization

Automatically categorizes emails into:

* Work
* College
* Personal
* Finance
* Promotional
* Other

### ✅ Task Extraction

Identifies meaningful actions the recipient is expected to perform.

### ⏰ Deadline Extraction

Extracts explicit deadlines without inventing missing information.

### 🛡️ Phishing & Spam Analysis

Analyzes suspicious signals including:

* Suspicious links
* Requests for sensitive information
* Financial requests
* Impersonation
* Artificial urgency
* Threats
* Sender inconsistencies

### 💬 Smart Reply Generation

Generates a concise, context-aware reply when responding would be useful.

### 🔍 Explainable AI

Important classifications are supported by evidence from the email rather than unexplained labels.

---

## 🧠 AI Output

MailMind produces structured JSON that can be consumed directly by the application.

```json
{
  "summary": "...",
  "priority": "high",
  "priority_reason": [],
  "category": "work",
  "tasks": [],
  "deadlines": [],
  "phishing_spam": {
    "classification": "safe",
    "reasons": []
  },
  "sentiment": "neutral",
  "reply": {
    "tone": "professional",
    "text": "..."
  }
}
```

This structured approach makes the AI output predictable, explainable, and easy to render in the frontend.

---

## 🖥️ Product Preview

### Main Dashboard

![MailMind AI Dashboard](./screenshots/dashboard.png)

### Email Analysis

![Email Analysis](./screenshots/email-analysis.png)

### Phishing Detection

![Phishing Detection](./screenshots/phishing-detection.png)

### Smart Reply

![Smart Reply](./screenshots/smart-reply.png)

> Screenshots will be added after the final interface is completed.

---

## 🔄 How It Works

```text
User Email
    ↓
Email Parsing
    ↓
AI Analysis
    ↓
┌─────────────────────────────┐
│ Summary                     │
│ Priority                    │
│ Category                    │
│ Tasks                       │
│ Deadlines                   │
│ Security Analysis           │
│ Sentiment                   │
│ Smart Reply                 │
└─────────────────────────────┘
    ↓
Actionable Email Intelligence
```

---

## 🧪 Example

### Input

> Your interview has been confirmed for tomorrow at 10:00 AM.
> Please review the role description and confirm your availability before 6 PM today.

### MailMind Output

**Priority:** 🔴 High

**Category:** Work

**Tasks:**

* Review the role description
* Prepare for the interview
* Confirm availability

**Deadline:**

* Today, before 6 PM

**Security:** 🟢 Safe

**Suggested Reply:**

> Hi Recruitment Team,
> Thank you for the confirmation. I confirm my availability for the interview tomorrow at 10:00 AM. I'll review the role description and prepare accordingly.
>
> Best,
> Ayushi

---

## 🛠️ Tech Stack

* **Frontend:** React / Next.js
* **Styling:** Tailwind CSS
* **AI:** LLM + Prompt Engineering
* **Backend:** `ADD_AFTER_BUILD`
* **Deployment:** `ADD_AFTER_BUILD`

---

## 🧩 Architecture

```text
                ┌──────────────────┐
                │     User Email   │
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │   Email Parser   │
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │    AI Engine     │
                └────────┬─────────┘
                         ↓
        ┌────────────────────────────────┐
        │ Structured Email Intelligence  │
        ├────────────────────────────────┤
        │ Summary                        │
        │ Priority                       │
        │ Category                       │
        │ Tasks                          │
        │ Deadlines                      │
        │ Phishing Analysis              │
        │ Sentiment                      │
        │ Smart Reply                    │
        └────────────────┬───────────────┘
                         ↓
                ┌──────────────────┐
                │   User Interface │
                └──────────────────┘
```

---

## 🏆 Why MailMind?

Most email tools focus on **summarization**.

MailMind focuses on **decision-making**.

The goal isn't simply to tell the user what an email says.

The goal is to tell them:

> **What should I understand, what should I do, and what should I be careful about?**

---

## 🔐 Safety & Reliability

MailMind is designed to avoid hallucinating important information.

The system:

* Does not invent deadlines
* Does not invent responsibilities
* Does not invent sender information
* Explicitly represents missing information
* Supports evidence-based classifications
* Treats suspicious financial and credential requests carefully

---

## 📈 Future Scope

Potential future improvements include:

* 🌍 Multi-language email analysis
* 😊 Sentiment analysis improvements
* 📅 Calendar event extraction
* 🎙️ Voice-based email summaries
* 🔔 Follow-up reminders
* ✏️ One-click reply customization
* 📥 Gmail / Outlook integration
* 📊 Email productivity analytics

---

## 👩‍💻 Built For

**PromptWars × GITM Coding Club**

Built with AI, prompt engineering, and a focus on solving a real productivity problem.

---

## 📄 License

This project is created for educational and hackathon purposes.
