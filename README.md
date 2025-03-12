# Supabase Nuxt Monorepo

A monorepo containing Nuxt applications with Supabase integration.

## Project Structure

- `/nuxt` - Nuxt 3 application (v3.16.0)
- `/supabase` - Supabase Docker setup for local development
- `/ui` (planned) - Shared UI components with Storybook

## Requirements

- Node.js 22
- pnpm
- Docker (for Supabase local development)

## Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   cd nuxt
   pnpm install
   ```
3. Start Supabase:
   ```bash
   cd supabase
   docker compose up -d
   ```
4. Access Supabase Studio at http://localhost:8000/?apikey=YOUR_ANON_KEY
   - Find your ANON_KEY in `supabase/.env`

5. Run the Nuxt app:
   ```bash
   cd nuxt
   pnpm dev
   ```

## Stopping Services

```bash
cd supabase
docker compose down
```