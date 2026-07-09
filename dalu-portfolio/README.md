# Dalu — Portfolio

A minimalist, whitespace-driven personal portfolio built with React, TypeScript,
Tailwind CSS, and Vite.

## Getting started

```bash
npm install
npm run dev
```

Then open the local URL Vite prints (usually `http://localhost:5173`).

## Build for production

```bash
npm run build
npm run preview
```

The production build is output to `dist/`.


## Project structure

```
src/
  components/
    Nav.tsx        — sticky nav, gains a border on scroll
    Hero.tsx        — asymmetric hero with stats
    About.tsx       — bio + three-pillar framing (Build / Design / Create)
    Work.tsx        — project grid (edit the PROJECTS array to update)
    Skills.tsx      — grouped skill list (edit SKILL_GROUPS to update)
    Contact.tsx     — contact links (edit CONTACT_LINES to update)
    Footer.tsx
  hooks/
    useReveal.ts    — IntersectionObserver-based scroll reveal
    useScrolled.ts  — tracks scroll position for the nav border
  index.css         — Tailwind directives + custom component classes
  App.tsx
  main.tsx
```

## What to customize before launch

- `src/components/Work.tsx` — swap in real project links, screenshots if you
  add an image field, and update descriptions as projects evolve.
- `src/components/Contact.tsx` — replace the placeholder email and GitHub URL
  with your real ones.
- `src/components/Hero.tsx` — update the stats (years building, projects
  shipped) as they change.
- `index.html` — update the `<title>` and consider adding meta tags for
  social sharing (Open Graph / Twitter card) once the site is live.
