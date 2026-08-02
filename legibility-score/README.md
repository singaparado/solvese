# The Legibility Score
### A Solvese Diagnostic Tool

**Live:** https://solvese.vercel.app/legibility-score  
**Owner:** Mahdi Singaparado / Solvese  
**Stack:** Static HTML, CSS, and JavaScript — no build step, no server, no dependencies

---

## What It Does

The Legibility Score is a real-time diagnostic engine that evaluates hero
copy for organizations operating in complex domains against the Three Laws
of Translation:

- **Tangibility** — Does a stranger know what changes for them?
- **Intuitiveness** — Does it read at the speed of thought?
- **Sustainability** — Does it frame the offering as an ongoing environment, not a one-off transaction?

Paste hero copy. Receive a 0–100 composite Legibility Score, an Interpretation
Window assessment (5-second first-sentence legibility), and per-law fracture
diagnostics explaining exactly where the narrative breaks down.

No signup. No server. No data collected. Runs entirely client-side.

---

## Repository Status

This tool was originally prototyped on the Ploy AI builder, then fully
reverse-engineered and reconstructed as static HTML after that platform
offered no export path. All scoring heuristics, signal vocabulary, fracture
messages, and diagnostic concepts were preserved exactly during that
reconstruction and are proprietary to Solvese.

---

## Scoring Methodology

The composite score weights:
- Tangibility: 34%
- Intuitiveness: 40%
- Sustainability: 26%

Three proprietary signal arrays drive detection: JARGON_SIGNALS,
OUTCOME_SIGNALS, and WORKFLOW_SIGNALS. An Interpretation Window check
additionally verifies that the first sentence stays at or under 18 words
with fewer than 2 jargon signals.

**Do not modify scoring constants without a deliberate recalibration pass —
they are the diagnostic's core IP.**

---

## Deployment

Deployed to Vercel as a static page. Connected to the main Solvese domain at
`solvese.vercel.app/legibility-score`.

---

## Intellectual Property

The Legibility Score methodology — including the Three Laws of Translation,
the Interpretation Window concept, signal vocabulary, fracture message
system, and scoring formulas — is proprietary intellectual property of
Solvese / Mahdi Singaparado. This repository exists to establish and
maintain source-level ownership of that IP.
