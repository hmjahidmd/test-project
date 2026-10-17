# test project

A Node.js web app by [hmjahid](https://github.com/hmjahid). The target stack is **TypeScript** and **Next.js** (App Router).

## Status

The repo is in an early setup stage. `package.json` is initialized and `dotenv` is installed. Next.js and TypeScript are not wired up yet.

## Tech stack

| Layer | Choice |
| --- | --- |
| Runtime | Node.js |
| Language | TypeScript |
| Framework | Next.js (App Router) |
| Env vars | `dotenv` |

## Requirements

- Node.js 18 or newer
- npm

## Setup

```bash
npm install
```

Copy environment variables into a `.env` file in the project root. Do not commit secrets.

## Scripts

| Script | Description |
| --- | --- |
| `npm test` | Placeholder (no tests yet) |

Dev and production scripts (`next dev`, `next build`, `next start`) will be added when Next.js is scaffolded.

## Project layout (planned)

```
app/           # Next.js App Router pages and route handlers
components/    # Shared UI
lib/           # Shared logic
types/         # Shared TypeScript types
```

## License

ISC
