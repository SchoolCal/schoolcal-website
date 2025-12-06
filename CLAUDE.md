# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

SchoolCal marketing website built with Next.js 15, React 19, and Tailwind CSS 4. Uses Sanity as a headless CMS.

## Commands

```bash
npm run dev      # Start development server (http://localhost:3000)
npm run build    # Production build
npm run lint     # Run ESLint
npm run start    # Start production server
```

## Architecture

- `app/` - Next.js App Router pages and components
  - `components/` - Shared React components (Header, Footer, forms, etc.)
  - `globals.css` - Design system with CSS variables and custom typography/color classes
- `lib/sanity.ts` - Sanity CMS client (requires `NEXT_PUBLIC_SANITY_PROJECT_ID`, `NEXT_PUBLIC_SANITY_DATASET`, `SANITY_API_READ_TOKEN`)

## Cursor Rules

See `.cursor/rules/` for detailed conventions:
- `server-side-rendering.mdc` - SSR requirements for SEO/LLM crawlability (critical)
- `website-design.mdc` - Design system: typography classes (`heading-1/2/3`, `body-large/medium/small`) and color classes
- `schoolcal-rules.mdc` - Tech stack choices (Tailwind, Sanity)
- `selecting-icons.mdc` - Use `lucide-react` for icons
- `meta-data.mdc` - Page metadata requirements
