# KAYVEN Capital OS

A private, premium investor-intelligence and fundraising pipeline web app for KAYVEN (kayven.ai).

## Tech Stack

- **Framework**: Next.js 16 (App Router) with TypeScript strict mode
- **Styling**: Tailwind CSS v4
- **Animations**: Framer Motion
- **Backend**: Supabase (PostgreSQL + Auth + Row Level Security + pgvector)
- **State Management**: React Context/Zustand (TBD)
- **Form Validation**: Zod
- **Table Component**: TanStack Table
- **Drag & Drop**: dnd-kit for Kanban
- **Testing**: Vitest + Playwright
- **Deployment**: Vercel with GitHub Actions CI

## Design System

- Minimalist Monochrome: pure black/white, high-contrast, restrained accent
- Serif display type + clean sans/mono for data
- Sharp corners, hairline borders, generous whitespace
- SVG icons only (Lucide or Phopshor, single weight, 1.5px stroke)
- Purposeful motion (150-250ms), respects prefers-reduced-motion
- Dark and light themes, WCAG AA compliant, responsive down to mobile

## Getting Started

### Prerequisites

- Node.js 20.x or later
- pnpm (recommended) or npm
- Supabase account

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pnpm install
   # or
   npm install
   ```
3. Copy `.env.example` to `.env.local` and fill in your Supabase credentials
4. Run the development server:
   ```bash
   pnpm dev
   # or
   npm run dev
   ```

### Environment Variables

Create a `.env.local` file with the following variables:

```
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
```

## Database Setup

Run the migration scripts in `/supabase/migrations` to set up the database schema.

## Development Guidelines

- Trunk-based development with short-lived branches (feat/, fix/, chore/, docs/)
- Conventional Commits
- Small atomic commits
- Squash-merge PRs via PR template
- No secrets committed - validate env with Zod at boot
- Real data only - never fabricate emails, contact details, or unverified claims
- Source attribution - every record stores its source; research cards cite every claim

## Milestones

See [PLAN.md](PLAN.md) for detailed implementation roadmap.

## License

Private/proprietary - All rights reserved.# Outreach
