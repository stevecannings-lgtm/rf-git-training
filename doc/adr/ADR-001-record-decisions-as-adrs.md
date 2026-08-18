# ADR-001: Record decisions as Architecture Decision Records

**Status:** Accepted
**Date:** 2026-08-11
**Decision makers:** Steve Cannings (Technical PM)

## Context

This repository is new. Right Formula's established codebases (Halo / `banger-events`) already keep Architecture Decision Records, and the habit has paid off: decisions made in meetings, chat threads and email are lost within weeks, while a decision written down next to the code survives team changes and — increasingly important — is visible to AI agents working in the repository, who will otherwise confidently re-litigate or overturn settled decisions.

As we bring more people (and agents) into repositories like this one, we need one obvious place where "what we decided, and why" lives.

## Decision

### 1. Keep ADRs in the repository, next to the code

Decision records live in `doc/adr/`, one Markdown file per decision, numbered sequentially:

```
doc/adr/ADR-001-record-decisions-as-adrs.md
doc/adr/ADR-002-<short-kebab-case-title>.md
```

### 2. Use a fixed, minimal format

Every ADR has the same skeleton (see the template at the end of this file):

- **Header** — number, title, status (`Proposed` / `Accepted` / `Superseded`), date, decision makers.
- **Context** — the situation and forces that made a decision necessary, written so a newcomer needs no other documents.
- **Decision** — what we chose, stated plainly in the present tense.
- **Consequences** — what gets easier, what gets harder, what we have knowingly accepted.
- **Options considered and rejected** — each rejected option with the reason it lost. This section is load-bearing: a rejected option recorded without its rejection reasoning invites someone (or some agent) to propose it again.

### 3. ADRs are living documents

An ADR always reflects our *current* understanding of one concern, not a history of our thinking:

- Refinements, extensions, clarifications — and even outright reversals — are **edits to the existing file**, not new files. Rewrite so the current position reads as the decision all along.
- History lives in `git log`, which is authoritative. Don't duplicate it into the ADR text.
- Start a new file only for a genuinely new topic.

### 4. What belongs in an ADR

Decisions whose consequences outlive the pull request: architecture, data shapes, naming conventions, tooling choices, ways of working. Anything obvious from reading the code itself does **not** need an ADR.

## Consequences

- New joiners and AI agents can read `doc/adr/` and learn both what we decided and why, without archaeology through old chats and tickets.
- Each significant decision costs a few minutes of writing. Experience on Halo shows this is repaid the first time anyone asks "why is it like this?".
- Challenging a decision is always welcome — the record exists to make the challenge well-informed, not to discourage it. A successful challenge ends with the ADR edited in place.

## Options considered and rejected

- **Wiki / SharePoint pages** — drift away from the code, are invisible to anyone (or any agent) working inside the repository, and rot silently. Rejected.
- **A decision-log spreadsheet** — same drift problem, a worse authoring experience, and no review step. Rejected.
- **Commit messages / PR descriptions only** — good history, terrible discoverability; nobody reads two years of log to learn a convention. Git stays authoritative for *history*; ADRs carry the *current state*. Rejected as the primary record.

---

## Appendix — template for a new ADR

Copy this into `doc/adr/ADR-NNN-short-title.md` and fill it in:

```markdown
# ADR-NNN: <Title — the decision in one line>

**Status:** Proposed
**Date:** YYYY-MM-DD
**Decision makers:** <names / roles>

## Context

<What situation forced a decision? What constraints and forces are in play?
Write it so a newcomer needs no other document.>

## Decision

<What we chose, plainly, in the present tense.>

## Consequences

<What gets easier, what gets harder, what trade-offs we knowingly accept.>

## Options considered and rejected

- **<Option>** — <why it lost>.
```
