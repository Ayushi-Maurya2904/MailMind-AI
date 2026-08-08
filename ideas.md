# MailMind AI — Design Direction

## Approach 1
**Theme Name:** Signal Desk

**Very Brief Intro:** A crisp editorial command center that turns messy inbox content into calm, prioritized decisions. Warm paper tones and sharp signal colors make important findings feel immediate without becoming alarmist.

**Probability:** 0.07

## Approach 2
**Theme Name:** Quiet Orbit

**Very Brief Intro:** A dark, atmospheric AI workspace with luminous data markers and a sense of protected focus. The visual language is observant and technical, using restrained glow only for meaningful system states.

**Probability:** 0.03

## Approach 3
**Theme Name:** Studio Inbox

**Very Brief Intro:** A playful, tactile productivity studio inspired by stationery, index cards, and highlighter marks. It makes analysis feel approachable and memorable while keeping the information hierarchy rigorous.

**Probability:** 0.09

## Selected Direction: Signal Desk

### Design Movement
Contemporary editorial software: the clarity of a modern newsroom desk combined with the precision of a lightweight operations console.

### Core Principles
1. **Signal over decoration:** every accent color communicates a real state such as priority, risk, or completion.
2. **Editorial hierarchy:** oversized headlines, compact metadata, and strong section labels let users scan before they read.
3. **Warm credibility:** parchment, ink, and cobalt create a human, trustworthy workspace instead of a sterile AI interface.
4. **Evidence beside recommendations:** extracted facts are visually separated from AI-generated guidance.

### Color Philosophy
A warm ivory canvas makes the app feel calm and readable, while near-black ink gives email content the gravity of a document. Cobalt is the ownable action color for analysis and focused state. Amber and coral are reserved for urgency and security risk; sage is reserved for safe/confirmed signals. The palette is intentionally low-saturation outside those signals so the important cards carry the visual energy.

### Layout Paradigm
A two-column command desk: a narrow navigation rail and a broad working canvas. The primary analysis flow sits in a slightly offset editorial column, with a specimen-like email input panel on the left and results that unfold in modular cards below. The interface should feel composed, not centered like a marketing landing page.

### Signature Elements
- A cobalt vertical signal rail on the left edge of the app shell.
- Tiny uppercase evidence labels such as `EXTRACTED FROM EMAIL` and `SAFE RECOMMENDATION`.
- Highlight-marker underlines and thin ruled dividers that echo an annotated briefing document.

### Interaction Philosophy
Interactions should feel like handling a well-made paper tool: immediate, tactile, and legible. Demo emails are quick-fill specimens, the primary button gives visible feedback, and result cards reveal in a measured cascade. No interaction should imply a real inbox connection.

### Animation
Use short 160–240ms ease-out transitions. The analyze action moves through a compact scanning state with a subtle pulsing signal dot. Results fade and rise in a staggered cascade. Hover states should lift cards by 2px and deepen their shadow; reduced-motion users receive instant transitions.

### Typography System
Use **DM Sans** for readable interface copy and **Space Grotesk** for display headlines, labels, and numeric signal values. Headlines use tight tracking and a confident weight; body copy stays at 15–16px with generous line height. Metadata is uppercase at 10–11px with deliberate letter spacing.

### Brand Essence
MailMind AI is an email-to-action assistant for students and early-career professionals who need clarity without losing context; it is different because it pairs structured extraction with safe, explainable recommendations.

**Personality:** observant, composed, practical.

### Brand Voice
Headlines are direct and slightly editorial. CTAs use active verbs. Microcopy explains why a result exists instead of overpromising intelligence.

- “Your inbox has too much noise. Find the signal.”
- “Read the evidence before you reply.”

### Wordmark & Logo
The mark is a compact cobalt square containing three offset white “signal lines” that rise from left to right, suggesting both an email stack and a thought becoming clear. The wordmark uses a custom-spaced `MailMind` lockup in Space Grotesk Semibold, with `AI` set in cobalt.

### Signature Brand Color
**Signal Cobalt — #3155D9.** A focused, reliable blue that feels more editorial than corporate and stays legible against warm ivory.

## Style Decisions
- Use the Signal Desk direction across the entire app; do not introduce dark neon or generic purple gradients.
- Keep extracted email facts and AI recommendations in visibly distinct visual treatments.
- Use generated visual assets only as quiet brand texture, never as a substitute for functional dashboard content.

## Style Decisions

- The app must expose a visible cobalt left signal rail or equivalent command-desk spine; centered marketing-page composition is not the default layout.
- Large decorative panels must contain product-relevant briefing content, evidence fragments, signal markers, or annotated email material.
- State colors are semantic only: cobalt means action/focus, coral means risk/security concern, amber means urgency, and sage means safe/confirmed.
- The hero now includes a miniature briefing preview so the product demonstrates its evidence/recommendation split before analysis.
