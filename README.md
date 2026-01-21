# Drift

A calm, open-source personal growth dashboard for developers.

Drift helps individuals notice momentum, catch drift, and stay intentional in their learning and projects — without pressure, gamification, or productivity theater.

![Open Source](https://img.shields.io/badge/open--source-yes-brightgreen)
![License](https://img.shields.io/github/license/vikz91/driftme)
![Bun](https://img.shields.io/badge/runtime-bun-black)
![React](https://img.shields.io/badge/frontend-react%2019-blue)
![Docker](https://img.shields.io/badge/container-docker-blue)
![Turborepo](https://img.shields.io/badge/monorepo-turborepo-purple)
![Status](https://img.shields.io/badge/status-active%20development-orange)


🌑 **Dark theme only**  
🧘 **Personal-first, no collaboration**  
🆓 **Free, open source, self-hostable**

👉 Repository: https://github.com/vikz91/driftme

---

## Status

> 🚧 Early-stage / active development

The core philosophy and structure are stable. Features will evolve conservatively.

---

## Tech Stack

### Backend
- **Bun** (runtime & package manager)
- **Hono** (HTTP framework)

### Frontend
- **React 19**
- **React Router v7**
- **react-router-dom**
- **SWR** (data fetching)

### UI
- **Tailwind CSS**
- **shadcn/ui**
- **Headless UI primitives**
- **Lucide Icons**

### Database
- **MongoDB**
- **Mongoose**

### Monorepo & Tooling
- **Turborepo**
- **Bun workspaces**

### DevOps
- **Docker**
- **Docker Compose** (aux services)
- **GitHub Actions** (CI)

### Code Quality
- **ESLint**
- **Prettier**
- **Husky**
- **lint-staged**

---

## Repository Structure

```

drift/
├─ apps/
│  ├─ web/          # Frontend (React)
│  ├─ api/          # Backend (Bun + Hono)
│
├─ packages/
│  ├─ ui/           # Shared UI components
│  ├─ config/       # Shared configs (eslint, ts, etc.)
│
├─ docker/
│  └─ docker-compose.yml
│
├─ PROJECT.md
├─ CONTRIBUTING.md
└─ turbo.json

````

Structure may evolve, but Drift will remain a **single monorepo**.

---

## Prerequisites

Ensure you have the following installed:

- **Bun** ≥ latest stable  
  https://bun.sh
- **Node.js** ≥ 18 (for tooling compatibility)
- **Docker** (optional, for DB & services)
- **MongoDB** (local or Docker)

---

## Getting Started

### Install dependencies

```sh
bun install
````

---

### Start development (all apps)

```sh
bun run dev
```

This runs all apps and packages via Turborepo.

---

### Start a specific app

```sh
bun run dev --filter=web
bun run dev --filter=api
```

---

### Build

```sh
bun run build
```

Or filtered:

```sh
bun run build --filter=web
```

---

## Environment Variables

Each app manages its own `.env` file.

Example (API):

```env
MONGODB_URI=mongodb://localhost:27017/drift
```

---

## Authentication

Drift supports:

* GitHub OAuth
* Google OAuth

Auth is required for the hosted version.
Self-hosted instances may adapt this as needed.

---

## Hosting

You can:

* Self-host Drift on your own infrastructure
* Use the free hosted version at **[https://drift.me](https://drift.me)**

Both provide the same feature set.

---

## Philosophy & Scope

Drift is intentionally:

* Personal, not social
* Reflective, not metric-driven
* Opinionated, not configurable
* Calm, not motivating through pressure

For full context, see **[PROJECT.md](./PROJECT.md)**.

---

## Contributing

Drift is open source and contributions are welcome, but the project is intentionally conservative.

Before contributing:
- Read [PROJECT.md](./PROJECT.md) to understand the philosophy
- Read [CONTRIBUTING.md](./CONTRIBUTING.md) for contribution rules
- Open an issue before proposing new features

Small, focused improvements are preferred over large changes.


---

## Issues & Feedback

Please use GitHub Issues for:
- Bug reports
- UX problems
- Clarification questions
- Feature discussions (proposal only)

Before opening an issue:
- Check existing issues
- Keep scope narrow
- Avoid feature requests that add pressure, noise, or complexity

See [ISSUES.md](./ISSUES.md) for guidelines.

---

## License

**AGPL-3.0-only**

You are free to:

* Use Drift
* Fork Drift
* Self-host Drift
* Modify Drift

Hosted derivatives must publish their source changes.

---

## Support

Drift is free and maintained as a public-good project.

If you find value in it:

* ⭐ Star the repo
* 🧩 Contribute code or docs
* ❤️ Support via GitHub Sponsors (optional)

---

## Guiding Question

Every change must answer:

> Does this help a developer understand their current growth state without increasing mental load?

If not, it does not belong in Drift.

