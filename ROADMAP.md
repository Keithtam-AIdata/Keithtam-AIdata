# AI + Data Portfolio Roadmap

**Owner:** Keith Tam — Data Analyst (Lifemark Health Group, Canada)
**Goal:**  Business-leaning **Applied AI / AI Solutions / AI-enabled Data** role.

---

## 1. Positioning — who this portfolio says I am

> A senior data professional (SQL · Power BI · Python, healthcare industry) who can
> **identify where AI creates business value, build the application, and prove it works** —
> not an LLM researcher, and not a 100% software developer.

Target titles: **Applied AI Engineer · AI Solutions Analyst · GenAI Engineer · AI-enabled Senior Data Analyst · Data & AI Consultant.**

The portfolio's only job is to close the one gap in my CV: my current role has no AI exposure. Everything below proves I can apply AI even though my day job can't.

---

## 2. Design principles (why the projects are chosen this way)

1. **One pattern per project.** Each project demonstrates a *different* enterprise-AI pattern, so the portfolio reads as a spectrum of capability — not the same OpenAI wrapper five times.
2. **Cross-industry on purpose.** Retail, finance, cross-functional ops, healthcare. Range signals adaptability; one healthcare project ties back to real domain experience.
3. **Depth beyond the wrapper.** Each project does the one thing that separates "I called an API" from "I understand the technique": eval harness, retrieval quality, SQL guardrails, tool orchestration.
4. **Senior signal = judgment + impact, not features.** Every README states the business problem, the trade-off I made, and a quantified impact — the questions a senior interview actually asks.
5. **Sustained cadence over a sprint.** Built across months with steady commits and milestone posts. A repo that keeps moving beats a repo finished in one weekend and abandoned.

---

## 3. The enterprise-AI pattern map (and my coverage)

| # | Pattern | What it does in a company | Covered by |
|---|---------|---------------------------|------------|
| 1 | Knowledge retrieval (RAG) | Q&A over internal docs / policies, with citations | Project 3 |
| 2 | Conversational analytics / text-to-SQL | Ask data in natural language, AI computes + explains | Project 2 (v2) |
| 3 | Internal copilot / assistant | Cross-tool employee assistant | (touched across) |
| 4 | Document intelligence / extraction | Unstructured docs → structured data | Project 5 |
| 5 | Agentic automation / workflow | Multi-step AI agent runs a process end to end | Project 4 |
| 6 | Content generation | Auto-draft reports, summaries, emails | (built into P2/P4) |
| 7 | AI reliability / eval / guardrails | Make LLM output accurate, safe, trustworthy | Project 2 & every project |

Today I cover ~1 of 7. The roadmap takes me to 4–5 well-covered patterns, with eval running through all of them as a differentiator.

---

## 4. The roadmap

> Status legend: ✅ done · 🔧 in progress · ⬜ planned

### Phase 0 — Foundation (done, Jun 2026)
**Project 1 — AI Business Insight Generator** ✅ — beginner project; Excel → KPIs → AI summary.
**Project 2 — Business Analytics Assistant (v1.1)** ✅ — pattern-driven dataset (6,912 rows, documented business patterns), KPI engine rewrite, analytics/UI split, consulting-grade redesign.

### Phase 1 — Jul–Aug 2026 · Project 2 → v2: Text-to-SQL + Eval
- **Pattern:** #2 conversational analytics + #7 reliability · **Industry:** retail / e-commerce
- **Upgrade:** replace keyword KPI engine with real **text-to-SQL** (AI writes SQL against DuckDB), add **SQL guardrails** (block dangerous / wrong queries), add an **eval harness** (a question→expected-answer set that scores accuracy on every change).
- **Senior signal:** "I don't just generate answers — I measure how often they're right, and I stop the model from running unsafe SQL."
- **Why first:** turns the existing flagship from a wrapper into a credible engineering artifact, and introduces a real database (DuckDB) as the light engineering backbone.

### Phase 2 — Sep–Oct 2026 · Project 3: RAG Knowledge Assistant
- **Pattern:** #1 knowledge retrieval · **Industry:** finance / insurance (e.g. policy & compliance docs) — deliberately a new sector
- **Build:** upload docs → chunk → embed → retrieve → answer **with citations**.
- **Depth beyond wrapper:** test **chunking strategies**, measure **retrieval quality** (did it fetch the right passage?), always show **source references**.
- **Senior signal:** "I can evaluate retrieval, not just bolt on a vector DB — and every answer is traceable to a source, which is what regulated industries require."

### Phase 3 — Nov–Dec 2026 · Project 4: Agentic Workflow Automation
- **Pattern:** #5 agentic automation · **Industry:** cross-functional analyst operations
- **Build:** an AI agent that runs a multi-step process end to end — e.g. ingest a raw file → run data-quality checks → generate a written report → flag anomalies — with **human-in-the-loop** approval.
- **Depth beyond wrapper:** **tool orchestration** (the agent calls multiple tools in sequence), guardrails, and a clear control flow.
- **Senior signal:** this is the portfolio's crown jewel — the least-common, most-in-demand pattern. "I can design an agent that *does* work, not just answers questions."

### Phase 4 — Jan–Feb 2027 · Project 5: Document Intelligence
- **Pattern:** #4 extraction · **Industry:** your choice — **healthcare** (ties to real domain) or **fintech** (e.g. invoice / claim / KYC document processing)
- **Build:** unstructured documents → structured fields → validation → export to a clean table.
- **Depth beyond wrapper:** **extraction accuracy eval**, handling messy / multi-format inputs, confidence scoring.
- **Senior signal:** "I can turn the unstructured-document problem — the one every bank and insurer has — into clean, validated data."

### Phase 5 — Feb–Mar 2027 · Polish & Launch
- Finalise every README as a **case study** (problem → architecture → decisions → impact).
- Architecture diagrams + decision logs across all projects.
- LinkedIn narrative finalised; CV / resume aligned to target titles.
- A pinned "portfolio overview" repo or profile README linking all five projects by pattern.

---

## 5. Sustained-cadence playbook (the part that proves persistence)

**GitHub — commit like a developer, not a dumper.**
- Never push a finished project in one commit. Stage it: `scaffold → data → core logic → eval → docs → polish`, each a meaningful commit message. The commit history then tells a development story.
- Aim for **2–4 meaningful commits per week**. A steadily green contribution graph over 9 months reads as "continuous learner."
- Use **GitHub Issues / Projects** to track this roadmap publicly — planning in the open is itself a senior signal.

**LinkedIn — one story, told in instalments.**
- Update headline + About now to the positioning in §1.
- Post at each milestone (~every 2–3 weeks): what I built, *why*, and one thing I learned. ~10–12 posts over 9 months.
- After each project, write one short case-study post linking the repo.
- Goal: by Mar 2027 a recruiter sees a 9-month arc of "senior analyst deliberately mastering applied AI," not a one-week dump.

**Monthly rhythm (repeat each phase):**
1. Week 1: scope + scaffold + open issues
2. Weeks 2–4: build core + eval, commit steadily
3. Week 5–6: docs, README case study, architecture diagram
4. End of phase: LinkedIn milestone post

---

## 6. Milestones at a glance

| Month | Deliverable | Pattern | Industry |
|-------|-------------|---------|----------|
| Jun 2026 | P2 v1.1 (data + UI) ✅ | analytics | retail |
| Jul–Aug | P2 v2 — text-to-SQL + eval | #2 + #7 | retail |
| Sep–Oct | P3 — RAG knowledge assistant | #1 | finance / insurance |
| Nov–Dec | P4 — agentic workflow automation | #5 | cross-functional ops |
| Jan–Feb | P5 — document intelligence | #4 | healthcare / fintech |
| Feb–Mar | Polish, case studies, LinkedIn, CV | — | — |

---

## 7. North star

> Use real data experience as the foundation; use AI to turn that experience into
> business-ready tools; prove every tool works. The portfolio shows applied,
> evaluated, business-grounded AI capability — sustained over time, not produced overnight.
