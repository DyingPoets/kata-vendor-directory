# Vendor Contact Directory — Schema + Work Orders

> **Branch:** `skill/schema-and-wos`
> **Skills:** A3 · W1 · R1 · R6
> **Audience:** PM · Eng

---

## For the Facilitator

### Session Overview

| | |
|---|---|
| **Kata** | 2: Vendor Contact Directory |
| **Session** | Schema + Work Orders |
| **Skills** | A3 · W1 · R1 · R6 |
| **Duration** | 2 hours (facilitated) + self-directed extension |
| **Slide Deck** | https://gamma.app/docs/mynxtnqxh6d1kc3 |
| **Miro Board** | https://miro.com/app/board/uXjVG8QBtVI%3D/ |

### Session Timing

| Time | Activity |
|------|----------|
| 0:00–0:15 | Concept framing — open the Gamma slide deck and walk through each slide |
| 0:15–0:30 | Orient to Miro board + this starting state |
| 0:30–1:05 | Step 1 exercise (Miro — Context frame) |
| 1:05–1:25 | Step 2 exercise (Miro — Exercise frame) |
| 1:25–1:30 | Step 3 wrap-up |
| 1:30–1:50 | Debrief — use Miro Debrief frame prompts |
| 1:50–2:00 | Extension brief — point to Extension Zone in Miro |

### What to Watch For

- WOs that are too large — anything over 4 hours is a red flag
- Schemas with no constraints (missing NOT NULL, no foreign keys) — push for real data modeling
- Participants who sequence WOs without drawing dependencies — make the dependency map explicit

### Facilitation Tips

- Ask "could this WO be tested by itself right now?" to validate decomposition
- Have teams swap WO lists and critique: "Which of these could run in parallel?"
- At debrief, highlight the best example of an independently deployable WO

### Extension / Coaching Office Hours

Participants can continue extension work independently and bring it to **Coaching Office Hours**.
At Office Hours, focus on: what decision did they make, why, and what would they change?

---

## For Participants (Developer · PM · UX)

### Getting Started

```bash
git clone https://github.com/DyingPoets/kata-vendor-directory
git checkout skill/schema-and-wos
```

Open the Miro board and the Gamma slide deck — have both visible during the session.

- **Slides:** https://gamma.app/docs/mynxtnqxh6d1kc3
- **Miro Board:** https://miro.com/app/board/uXjVG8QBtVI%3D/

### What You'll Practice

- A3
- W1
- R1
- R6

### Your Starting State

You have:
- `requirements/feature-list.md` — the facilities manager's feature wishlist
- `wireframes/vendor-directory-sketch.md` — a rough description of the UI

Your goal: design the Vendor entity schema and break the feature into 5–8 Work Orders.

### Step by Step

**Step 1:** Read the feature list and wireframe. Design the Vendor entity: fields, types, constraints, indexes. Consider: search, bulk export, change history.

**Step 2:** Decompose the feature into 5–8 WOs. Each WO must be: independently testable, under 4 hours, named as an outcome (not a task).

**Step 3:** Draw a dependency map. Identify which WOs can run in parallel. Which is the critical path?

### What Good Looks Like

A schema with real constraints and a WO list where every item could be demo'd to a stakeholder independently on day one of delivery.

See the `solutions/` directory for reference examples — but try the exercise first.

### Extension Work

- Add a vendor-contact change-history design: who changed what field, when, and from what value
- Map your WOs to a 2-week sprint — which ones are blocked? Which ones can start immediately?
- Write acceptance criteria for WO 1 in Gherkin format

Bring your extension work to **Coaching Office Hours**. You'll get 15 minutes of focused feedback.

---

Part of the [PDLC Training Katas](https://github.com/DyingPoets) series.
