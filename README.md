# Strata

**One engine, two adapters — a worked Forward Deployed scenario.**

Strata is an interactive walkthrough of a GenAI roadmap that turns unstructured input into structured
records, with a human on *only* the uncertain cases. One extraction engine is built once — ingest →
extract (LLM, logprobs on) → per-field confidence → validate → confidence router → auto-write or human
review → nightly eval loop — and a different adapter sits in front of it per domain:

- **UC1 — Scheduling intake:** email / text → structured scheduling rows.
- **UC2 — Acquisition integration:** scanned paper → structured records (vision-LLM, with typed-vs-handwritten
  conflict detection).

Flip the adapter toggle and watch the same engine handle a different input.

## Real vs. simulated
- **Real:** the workflows and the analysis - from two separate 40-minute interviews with operators who
  have 35+ years inside the company, plus three summers I worked in its branches.
- **Genericized:** the installer is a real company, deliberately unnamed; anything that would identify
  it - figures, system names, places, people - is removed or rounded.
- **Illustrative:** no engagement happened - this is a worked example - and there is no live AI; the
  demo plays back pre-written results to show how the work would flow.

## Build
Vanilla HTML/CSS/JS — a single self-contained `index.html`, no build step, no backend. Deployed static to
Vercel. Shares the portfolio's design system (dark forest, cream nodes, Fraunces / Inter / JetBrains Mono)
for cohesion when embedded.

---
A worked Forward Deployed scenario by Michael Cerpa.
