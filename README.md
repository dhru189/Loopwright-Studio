# Loopwright Studio

AI agent studio built with Next.js, Tailwind CSS, and shadcn/ui.

## Live Demo

**https://w1j6z9gyfb21-d.space-z.ai/**

## Features

- Multi-panel agent interface (Chat, Vision, Image generation, Search, TTS/Voice, Files)
- Project management
- WebSocket examples
- Prisma database schema
- Token Factory / ZAI integration ready (`src/lib/zai.ts`)

## Tech Stack

- Next.js (App Router)
- TypeScript
- Tailwind CSS + shadcn/ui
- Prisma
- Bun

## Getting Started

```bash
# Install dependencies
bun install

# Set up environment
cp .env.example .env   # add your keys

# Database
bun run db:generate
bun run db:push

# Development
bun run dev
```

## Project Structure

- `src/app` – pages and API routes (agent chat, vision, image, search, tts, projects)
- `src/components/loopwright` – main UI panels
- `src/components/ui` – shadcn components
- `src/lib` – utilities, db, store, zai client
- `prisma` – schema
- `examples/websocket` – websocket demo

## Notes

- `.env` is gitignored. Never commit secrets.
- This repository was initialized from the Loopwright workspace export.
