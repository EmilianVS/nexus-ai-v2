# 🧠 Nexus AI

A production-grade AI coding assistant. Powered by **DeepSeek**, synced via **Supabase Realtime**, with **GitHub App** private-repo access and **MCP** tool support.

## Stack
- **Frontend**: Next.js 15, Tailwind CSS, shadcn-style components
- **Backend**: FastAPI, SSE streaming, Redis rate limiting
- **Database**: Supabase (Postgres + RLS + Realtime)
- **AI**: DeepSeek V3 / R1 via OpenAI-compatible API
- **Auth**: Supabase Auth (email + OAuth)
- **GitHub**: GitHub App installation tokens (private repo access, no PAT needed)
- **MCP**: Model Context Protocol server proxy

## Quick Start

```bash
git clone https://github.com/EmilianVS/nexus-ai-v2
cd nexus-ai-v2
cp backend/.env.example backend/.env
cp frontend/.env.local.example frontend/.env.local
# Fill in values, then:
docker compose up --build
```

Open http://localhost:3000

## Deploy
| Service | Platform |
|---|---|
| Frontend | Vercel (root: `frontend`) |
| Backend | Railway / Render / Fly.io |
| Redis | Upstash |
| Database | Supabase (managed) |
