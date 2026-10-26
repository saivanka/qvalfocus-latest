# QvalFocus

An enterprise consulting website for QvalFocus, a global technology transformation firm: it presents the company's services and includes a backend for contact form submissions and newsletter subscriptions, with form spam protection.

## What it does

- Consulting-services website with a React frontend and an Express backend
- REST endpoints for contact form submissions and newsletter subscriptions
- Form protection via honeypot fields, CSRF protection and server-side Zod validation
- SEO via meta tags, OpenGraph cards and JSON-LD structured data; dark mode support
- An admin portal for career listings was added in later commits

## Tech stack

- Frontend: React 18 + TypeScript + Vite, Wouter routing, shadcn/ui on Radix UI primitives, Tailwind CSS, TanStack Query, React Hook Form + Zod
- Backend: Express.js + TypeScript (ES modules), PostgreSQL session storage via connect-pg-simple
- Data: PostgreSQL (Neon serverless) with Drizzle ORM and Drizzle Kit migrations

## How to run

```bash
npm install
npm run dev     # NODE_ENV=development tsx server/index.ts
npm run build   # vite build + esbuild server bundle
npm start       # NODE_ENV=production node dist/index.js
npm run check   # tsc
npm run db:push # drizzle-kit push
```

## Project structure

```
client/            # React frontend
server/            # Express backend (server/index.ts entry point)
shared/            # Shared code between client and server
replit.md          # Project overview and architecture notes
AI_RULES.md        # Project rules for AI-assisted edits
attached_assets/   # Static assets
```
