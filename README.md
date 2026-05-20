# SkillPilotAI

SkillPilotAI is a production-ready React + TypeScript app that creates career roadmaps with course links, beginner projects, progress tracking, profile/auth flows, and PDF export.

## Stack

- React + TypeScript + Vite
- React Router
- Tailwind CSS
- Shadcn-style Radix UI primitives
- Framer Motion
- Lucide Icons
- Supabase auth/database with local demo fallback

## Setup

1. Install dependencies:

   ```bash
   npm install
   ```

2. Copy environment variables:

   ```bash
   cp .env.example .env
   ```

3. Add Supabase values in `.env`:

   ```bash
   VITE_SUPABASE_URL=your-project-url
   VITE_SUPABASE_ANON_KEY=your-anon-key
   ```

4. Run the Supabase migration in `supabase/migrations` to create the `roadmaps` table and row-level security policies.

5. Start development:

   ```bash
   npm run dev
   ```

The app also works in demo mode without Supabase keys. Demo auth and roadmaps are stored in the browser, which is useful for local UI testing.

## AI Generation

By default the app uses a deterministic beginner-friendly roadmap generator so the UI works immediately. To connect a real AI backend, set:

```bash
VITE_AI_ENDPOINT=https://your-api.example.com/generate-roadmap
VITE_AI_API_KEY=optional-token
```

The endpoint should accept `{ "career": "Data Scientist" }` and return the roadmap shape defined in `src/types/roadmap.ts`.

## Scripts

- `npm run dev` - start the Vite dev server
- `npm run build` - type-check and build for production
- `npm run preview` - preview the production build
- `npm run lint` - run ESLint
- `npm run format` - format the project

## Features

- Landing page with original SkillPilotAI hero, quick picks, feature cards, and CTA flow
- Sign in/sign up, Google sign-in, protected routes, and profile
- Dashboard with roadmap generation, saved roadmaps, delete actions, and loading states
- Full roadmap page with XP, level unlocking, progress persistence, course/project cards, skills, interview prep, and PDF download
- Responsive layouts for mobile, tablet, and desktop
- SEO metadata, favicon, code splitting, and reusable services/components
