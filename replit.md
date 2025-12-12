# Aymaan Shahzad Portfolio Website

## Overview
A modern, minimal personal portfolio website built with React, TypeScript, and Tailwind CSS. Features dark mode toggle, responsive design, and a contact form.

## Project Structure
```
├── client/src/
│   ├── components/          # All section components
│   │   ├── Navigation.tsx   # Sticky header with nav links & theme toggle
│   │   ├── Hero.tsx         # Landing section with CTA buttons
│   │   ├── About.tsx        # Bio and summary
│   │   ├── Experience.tsx   # Timeline of work experience
│   │   ├── Projects.tsx     # Project cards with metrics
│   │   ├── Skills.tsx       # Categorized skill badges
│   │   ├── Education.tsx    # Academic background
│   │   ├── Contact.tsx      # Form with validation
│   │   └── Footer.tsx       # Copyright
│   ├── lib/
│   │   ├── portfolio-data.ts    # ALL PORTFOLIO CONTENT (edit this to update)
│   │   └── theme-provider.tsx   # Dark/light mode context
│   └── App.tsx              # Main app composition
├── server/
│   └── routes.ts            # Contact form API endpoint
└── README.md                # User documentation
```

## Key Files to Edit
- **Content**: `client/src/lib/portfolio-data.ts` - All personal info, experience, projects, skills
- **Styling**: `client/src/index.css` - Theme colors (uses Inter font, blue accent)
- **SEO**: `client/index.html` - Meta tags, title

## Tech Stack
- Frontend: React + TypeScript + Tailwind CSS + shadcn/ui
- Backend: Express.js (contact form API)
- Form: React Hook Form + Zod validation

## Running
- `npm run dev` starts both frontend (Vite) and backend (Express) on port 5000

## Recent Changes
- December 2024: Initial build with all core sections
- Dark mode with localStorage persistence
- Responsive mobile-first design
- Contact form with backend API
