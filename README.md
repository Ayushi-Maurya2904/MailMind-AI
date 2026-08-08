# 🧠 MailMind AI

> **Turn inbox noise into clear, actionable decisions.**

MailMind AI is an AI-powered email intelligence assistant that transforms unstructured emails into concise summaries, priority signals, actionable tasks, deadlines, security insights, and context-aware reply suggestions.

Built for the **PromptWars × GITM Coding Club** challenge.

---

## 🚀 Live Demo

**MailMind AI is deployed and ready to try.**

👉 Open the live application from the repository's deployment link.

---

## 🖥️ Preview

![MailMind AI Homepage](./homepage.jpg)

---

## 🎯 Problem

Professionals and students receive a large number of emails every day.

Important information can easily get buried among:

* Long messages
* Routine notifications
* Promotional emails
* Urgent requests
* Deadlines
* Potential phishing attempts

Manually reading, prioritizing, and organizing every email is time-consuming and can lead to missed tasks or delayed responses.

---

## 💡 Solution

**MailMind AI** converts an email into a structured decision layer.

Instead of simply asking:

> "What does this email say?"

MailMind asks:

> **"What does this email mean, what requires my attention, and what should I do next?"**

---

## ✨ Core Features

### 📧 Email Summarization

Converts lengthy emails into concise summaries while preserving important context.

### 🚨 Priority Detection

Classifies emails as:

* 🔴 High
* 🟡 Medium
* 🟢 Low

Priority is determined using evidence such as urgency, deadlines, required actions, consequences, and context.

### 🏷️ Smart Categorization

Each email is classified into one category:

* Work
* College
* Personal
* Finance
* Promotional
* Other

### ✅ Task Extraction

Identifies meaningful actions the recipient is expected to perform.

### ⏰ Deadline Extraction

Extracts explicitly stated deadlines without inventing dates or assumptions.

### 🛡️ Phishing & Spam Analysis

Analyzes signals such as:

* Suspicious links
* Requests for sensitive information
* Financial requests
* Impersonation
* Artificial urgency
* Threats
* Unusual requests
* Sender inconsistencies

### 💬 Smart Reply Generation

Generates concise, context-aware replies when a response would reasonably be useful.

### 🔍 Explainable AI

Important classifications are accompanied by evidence from the original email rather than unsupported guesses.

---

## 🧠 AI Output

MailMind produces structured output containing:

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

This structured approach makes the AI output easier to display, validate, and use inside the application.

---

## 🔄 User Flow

```text
Paste Email
     ↓
MailMind AI Analysis
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
User decides what to do next
```

---

## 🏗️ Architecture

```text
                ┌──────────────────┐
                │    User Email    │
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │  MailMind Input  │
                └────────┬─────────┘
                         ↓
                ┌──────────────────┐
                │   AI Analysis    │
                │   + Prompting    │
                └────────┬─────────┘
                         ↓
        ┌─────────────────────────────────┐
        │ Structured Intelligence Layer   │
        ├─────────────────────────────────┤
        │ Summary                         │
        │ Priority                        │
        │ Category                        │
        │ Tasks & Deadlines               │
        │ Phishing / Spam                 │
        │ Sentiment                       │
        │ Reply Generation                │
        └────────────────┬────────────────┘
                         ↓
                ┌──────────────────┐
                │  Actionable UI   │
                └──────────────────┘
```

---

## 🧪 Demo Scenarios

MailMind was tested against different types of emails, including:

### 1. Interview Confirmation

The system identifies:

* High priority
* Work category
* Interview preparation tasks
* Explicit confirmation deadline
* Professional reply requirement

### 2. Suspicious Payment Email

The system identifies:

* High priority
* Finance category
* Suspicious billing request
* Artificial urgency
* Suspicious domain/link
* Potential phishing risk

### 3. Normal / Low-pressure Email

The system distinguishes routine communication from genuinely urgent messages instead of simply reacting to words such as *"urgent"* or *"important"*.

---

## 🔐 AI Safety Principles

MailMind follows several important principles:

* **Evidence over assumptions**
* Never invent deadlines
* Never invent names or responsibilities
* Missing information is represented explicitly
* Dangerous classifications require multiple supporting signals
* Replies should not make unauthorized commitments
* Security recommendations should avoid directing users toward suspicious links

---

## 🛠️ Technology

* **TypeScript**
* **React**
* **Vite**
* **AI / Prompt Engineering**
* **Manus**
* Modern web UI components
* Structured JSON-based AI output

---

## 📁 Project Structure

```text
MailMind-AI/
│
├── client/
│   ├── public/
│   └── src/
│
├── server/
│
├── shared/
│
├── README.md
├── package.json
├── pnpm-lock.yaml
└── vite.config.ts
```

---

## 🎨 Design Philosophy

MailMind is designed around one idea:

> **Reduce cognitive load, not just email length.**

The interface separates:

* What the email says
* What matters
* What needs action
* What might be dangerous
* What the user can do next

The visual language intentionally uses clear hierarchy and signal-based UI rather than overwhelming the user with raw AI output.

---

## 🏆 Why MailMind?

Most email AI tools focus primarily on **summarization**.

MailMind goes one step further:

**Email → Understanding → Prioritization → Action → Decision**

The goal is not to make users read AI-generated text.

The goal is to help them **make a better decision faster.**

---

## 🔮 Future Scope

Potential future improvements include:

* 🌍 Multi-language email analysis
* 😊 Sentiment analysis improvements
* 📅 Calendar and meeting extraction
* 🔔 AI-powered follow-up reminders
* 🎙️ Voice-based email summaries
* ✏️ One-click reply customization
* 📬 Inbox integrations
* 🔐 More advanced phishing detection
* 📊 Personal email productivity analytics

---

## 👩‍💻 Built By

**Ayushi Maurya**

Built from scratch as a PromptWars × GITM Coding Club project.

---

## 📌 Project Status

**Prototype / Hackathon Submission**

The current version demonstrates the core MailMind intelligence workflow through a functional web application and structured AI analysis.

---

### ⭐ If you found the idea interesting, consider starring the repository.
