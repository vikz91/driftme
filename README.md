# Drift

A calm, open-source personal growth dashboard for developers.

Drift helps individuals notice momentum, catch drift, and stay intentional in their learning and projects — without pressure, gamification, or productivity theater.

🌑 **Dark theme only**  
🧘 **Personal-first, no collaboration**  
🆓 **Free, open source, self-hostable**

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

Contributions are welcome, but Drift is intentionally conservative.

Before contributing:

* Read **CONTRIBUTING.md**
* Open an issue for feature discussion
* Keep PRs small and focused

Philosophy alignment matters more than feature velocity.

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

```

---

### Why This README Works

- Removes Turborepo boilerplate noise
- Clearly states **what Drift is and is not**
- Signals seriousness to contributors
- Matches your OSS + free philosophy
- Scales with the project without rewriting later