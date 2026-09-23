# Katie Kanaan Portfolio

> A professional portfolio site for a medical student, covering education,
> clinical experience, research publications, and volunteer work.

**Live demo:** https://katie-k.vercel.app

## Overview

A single-page portfolio built for Katie Kanaan, a medical student at the
University of Iowa Carver College of Medicine. Experience entries — research
publications, clinical roles, and volunteer work — are stored as structured data
and rendered into a browsable carousel, each linking out to the source
publication or organisation. The site also serves her CV as a download.

## Features

- **Data-driven experience cards.** Entries live in a single `data.json` file
  and are tagged by category (Research Publication, Work, Volunteer), so adding
  an entry is a data change rather than a code change.
- **Carousel navigation** through experience entries, built on Embla Carousel.
- **Scroll-triggered fade-ins** via `IntersectionObserver`, animating each
  section in once as it enters the viewport.
- **CV download** and direct email and phone contact links.
- **Installable.** A web app manifest, icon set, and theme colour make the site
  installable to a home screen.
- **Custom error, loading, and not-found states** using the App Router's
  built-in boundary conventions.

## Tech stack

Next.js 16 (App Router) · React 18 · TypeScript · Tailwind CSS · shadcn/ui and
Radix primitives · Embla Carousel · Lucide icons · deployed to Vercel.

## Getting started

```sh
cd app
npm install
npm run dev
```

The site is fully static — no environment variables or backend services are
required.

## Project structure

```
app/src/
  app/         layout, page, data.json, boundary states
  components/  UI primitives (shadcn/ui) and shared components
  lib/         utilities
app/public/    images, icons, CV
```

## Scripts

| command | what it does |
|---|---|
| `npm run dev` | start the dev server |
| `npm run build` | production build |
| `npm run start` | serve the production build |
| `npm run lint` | ESLint |

## Credits

Site built by Noah Erickson. All biographical content, photographs, and CV
material belong to Katie Kanaan and are not covered by the licence below.

## License

The source code is released under the [MIT License](LICENSE).
