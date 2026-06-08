# Strata

**One engine, two adapters — a Forward Deployed case study.**

Strata is an interactive walkthrough of a GenAI roadmap that turns unstructured input into structured
records, with a human on *only* the uncertain cases. One extraction engine is built once — ingest →
extract (LLM, logprobs on) → per-field confidence → validate → confidence router → auto-write or human
review → nightly eval loop — and a different adapter sits in front of it per domain:

- **UC1 — Scheduling intake:** email / text → structured scheduling rows.
- **UC2 — Acquisition integration:** scanned paper → structured records (vision-LLM, with typed-vs-handwritten
  conflict detection).

Flip the adapter toggle and watch the same engine handle a different input.

## Real vs. simulated
- **Real:** the workflow, the architecture, the operator interviews, and the analysis behind it.
- **Sanitized:** the client, people, internal systems, and exact financials are genericized — no real company
  or product is named.
- **Illustrative:** there is no live AI here; the traces are scripted to show the routing.

## Build
Vanilla HTML/CSS/JS — a single self-contained `index.html`, no build step, no backend. Deployed static to
Vercel. Shares the portfolio's design system (dark forest, cream nodes, Fraunces / Inter / JetBrains Mono)
for cohesion when embedded.

---
Forward Deployed case study by Michael Cerpa.
