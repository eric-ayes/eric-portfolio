# Eric Ayestaran — Portfolio

Built with [Astro](https://astro.build) · Deployed on [Vercel](https://vercel.com)

## Setup

```bash
npm install
npm run dev       # localhost:4321
npm run build     # production build → dist/
npm run preview   # preview production build
```

## Deploy to Vercel

```bash
# Option A — Vercel CLI
npm i -g vercel
vercel

# Option B — Connect GitHub repo in vercel.com dashboard
# Push to GitHub → import repo → auto-deploy
```

## Connect your domain

1. Buy `ericayestaran.dev` via GitHub Student Pack (Namecheap)
2. In Vercel dashboard → Settings → Domains → Add `ericayestaran.dev`
3. Copy the DNS records Vercel gives you
4. In Cloudflare (after transferring) → DNS → paste records
5. Done in ~5 minutes

## Structure

```
src/
  components/
    Nav.astro        # Navigation + language toggle
    Hero.astro       # Hero section
    Projects.astro   # Project grid
    About.astro      # About + skills + timeline
    Contact.astro    # Contact block
    Footer.astro
  layouts/
    Base.astro       # HTML shell, cursor, scroll reveal
  pages/
    index.astro      # Main page + i18n script
  styles/
    global.css       # Design tokens, reset, cursor, animations
  data.js            # All content: projects, personal info, i18n strings
```

## Customization

- **Content** → edit `src/data.js`
- **Colors** → edit CSS variables in `src/styles/global.css` (`:root`)
- **New project** → add entry to `projects` array in `data.js`
- **New section** → create `src/components/NewSection.astro`, import in `index.astro`
