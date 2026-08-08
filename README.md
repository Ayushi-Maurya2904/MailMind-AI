# MailMind AI

MailMind AI is a static React MVP that turns a pasted email into a structured, actionable briefing. It is designed for a live college hackathon demo and does not claim access to a real inbox, Gmail, or any external integration.

## Features

- Paste or type an email into the analysis workspace.
- Analyze against the MailMind JSON contract: summary, priority, reasons, category, tasks, deadlines, phishing/spam classification, sentiment, and suggested reply.
- View results in a responsive dashboard instead of raw JSON.
- Clearly separates extracted email facts from AI-generated safe recommendations.
- Includes three immediately usable specimens: interview confirmation, suspicious Spotify/payment message, and a low-priority newsletter.
- Includes empty, loading, and validation/error states.
- Applies safety rules for untrusted email content. Suspicious messages never receive a suggested reply and show an official-channel verification recommendation.

## Run locally

```bash
pnpm install
pnpm dev
```

Then open the local Vite URL printed in the terminal. For a production build:

```bash
pnpm build
pnpm start
```

Type checking is available with `pnpm check`.

## Architecture

This is intentionally a frontend-only project. The main experience lives in `client/src/pages/Home.tsx`, where the interface, demo specimens, schema types, state machine, and isolated mock model adapter are easy to inspect. Shared UI primitives come from the scaffold’s shadcn/ui component set.

The analysis adapter is the `analyzeWithMockModel(email)` function in `Home.tsx`. It currently uses deterministic keyword/context matching so the demo works without an API key. To connect a real model later, replace that function with a server-side request that sends the MailMind Master Prompt V2, validates the returned JSON, and falls back to a safe error state for malformed responses. API keys must never be placed in frontend code.

## Output contract

The mock adapter returns the exact required object shape:

```json
{
  "summary": "string",
  "priority": "low | medium | high",
  "priority_reason": ["string"],
  "category": "work | college | personal | finance | promotional | other",
  "tasks": [{ "task": "string", "deadline": "string or null" }],
  "phishing_spam": {
    "classification": "safe | suspicious | dangerous",
    "reasons": ["string"]
  },
  "sentiment": "positive | neutral | negative | urgent | concerned",
  "reply": { "tone": "professional | friendly | concise | formal", "text": "string" }
}
```

`reply` is allowed to be `null` when no response is appropriate.

## Safety behavior

Email content is treated as untrusted data. The UI does not execute or follow instructions contained in the email. For the suspicious payment specimen, the app explicitly says not to click the link or share verification codes, passwords, OTPs, or banking credentials, and recommends checking only through the organization’s official app or website.

## Visual direction

The interface follows the **Signal Desk** system documented in `ideas.md`: warm editorial surfaces, Space Grotesk display typography, DM Sans body copy, Signal Cobalt action states, and visual evidence/recommendation separation.
