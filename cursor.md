# Cursor project notes

This is a Node.js app using TypeScript and Next.js. Use this file as persistent context for Cursor.

## Project

- Name: test project
- Owner: jahid (software engineer)
- Runtime: Node.js
- Language: TypeScript
- Framework: Next.js (App Router)

## Tech stack

- Node.js for the runtime and tooling
- TypeScript everywhere (app, config, and scripts) — avoid adding new `.js` files
- Next.js App Router (`app/`) with React Server Components by default
- Use Client Components (`"use client"`) only when browser APIs, local state, or event handlers are required
- Styling: CSS modules or Tailwind if the project already uses them; do not mix extra CSS frameworks without asking
- API routes / Route Handlers in `app/api/` when a backend endpoint is needed

## TypeScript

- Strict TypeScript. Prefer explicit types on public APIs; infer locally when it stays clear
- Do not use `any`. Use `unknown` and narrow, or a precise type
- Prefer `interface` for object shapes and `type` for unions, tuples, and mapped types
- Colocate types with the module unless they are shared — then put them in a `types/` folder

## Next.js conventions

- File-based routing only under `app/`
- Use `page.tsx`, `layout.tsx`, `loading.tsx`, and `error.tsx` as needed
- Fetch data on the server in Server Components or Route Handlers
- Use `next/link` for internal navigation and `next/image` for images
- Keep secrets in environment variables (`NEXT_PUBLIC_` only for values that must reach the browser)

## Agent preferences

- Work directly in code: create, debug, and iterate
- Prefer small, focused changes over large refactors
- Do not commit unless explicitly asked
- When changing UI, layout, routing, or client state, verify the flow in the browser before calling the work done

## Conventions

- Match existing file structure and naming before introducing new patterns
- Put shared UI in `components/`, shared logic in `lib/`
- Put Cursor rules in `.cursor/rules/` if they should always apply to the agent
