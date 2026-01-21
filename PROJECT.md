# Drift

A calm, personal growth dashboard for developers.

Drift helps individuals notice momentum, catch drift, and stay intentional in their learning and projects—without pressure, gamification, or productivity theater.

**Domain**: https://drift.me  
**Theme**: Dark-only  
**Audience**: Individual developers  
**Collaboration**: None (by design)

---

## Philosophy

Drift is intentionally **not** a productivity tool.

It exists to support *reflection*, not optimization.

Drift prioritizes:
- State over activity
- Momentum over metrics
- Intent over output
- Simplicity over configurability

Drift should feel like:
> Checking the current state of your growth—not managing it.

---

## Core Principles

1. **Free by default**  
   All features are available to everyone. No paywalls, tiers, or artificial limits.

2. **Open by design**  
   Drift is fully open source, forkable, and self-hostable.

3. **Personal-first**  
   Drift is built for individuals. There are no collaborative or social features.

4. **Opinionated simplicity**  
   Structure guides behavior. Fewer choices lead to clearer thinking.

5. **Calm UX**  
   No gamification, no streak pressure, no engagement traps.

---

## Access & Hosting

Drift can be used in two equally valid ways:

### Self-hosted
- Full functionality
- No restrictions
- Run locally or on your own infrastructure

### Hosted (drift.me)
- Free to use
- Best-effort availability
- Same feature set as self-hosted

Authentication:
- GitHub OAuth
- Google OAuth

Drift does not:
- Enforce usage limits
- Restrict features
- Lock users into the hosted version

---

## Application Structure

Drift consists of a small set of focused pages.

### Dashboard (Primary)
Mobile-friendly and designed for frequent use.

- Today’s focus (single intent)
- Momentum snapshot (human-readable state)
- Active projects (Hot/Warm only)
- Skill temperature overview
- Foundations pulse (DSA & System Design)

---

### Projects
Personal projects as growth vehicles.

Each project includes:
- Name and short description
- Status: Hot / Warm / Cold / Glacier
- Next tiny step (single field)
- Links (GitHub, demo, docs)
- Skills used
- Optional screenshots

Read-only GitHub integration:
- Repository link
- Open PR count
- Last commit timestamp

---

### Skills
Long-term capability tracking.

Each skill includes:
- Temperature state
- Subjective confidence rating
- Single active focus area
- Linear roadmap visualization

Only one roadmap node can be active at a time.

---

### Foundations
Evergreen fundamentals.

#### DSA
Tracked by concept exposure, not problem count.

#### System Design
Tracked by patterns, not system builds.

Both use simple states:
- Active
- Touched
- Untouched

---

## UI & UX Constraints

- Dark theme only
- Monochrome palette with one accent color
- System font
- Inline editing
- Keyboard-friendly
- Minimal animations (state transitions only)

The dashboard must remain mobile-friendly at all times.

---

## Sustainability

Drift is maintained as a public-good project.

There is no obligation to pay to use Drift.

Support is optional and voluntary:
- Code contributions
- Documentation improvements
- Design feedback
- Donations (e.g. GitHub Sponsors)

---

## Non-Goals

Drift explicitly does not aim to:
- Maximize engagement
- Track time or sessions
- Optimize productivity metrics
- Compete with task managers
- Provide collaboration or social features
- Act as a commercial SaaS

If a feature introduces pressure, noise, or obligation, it does not belong in Drift.

---

## Guiding Question

Every design and engineering decision must answer:

> Does this help a developer understand their current growth state without increasing mental load?

If the answer is no, the feature should not exist.
