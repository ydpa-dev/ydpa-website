# Youth Drug Protection Alliance — website

A 4-page static site: `index.html` (home), `about.html`, `initiatives.html`,
`contact.html`. No build step, no framework — plain HTML, CSS, and a small JS
file for the mobile nav, so it deploys on Vercel with zero configuration.

## Design system

- **Colors** (sampled directly from the approved mockups):
  sand `#EDE0D4` · white `#FFFFFF` · footer brown `#3A1D09` ·
  purple accent `#806490` · rust body text `#775332` · near-black headings `#0A0A0A`
- **Fonts**: Playfair Display (headings) + Inter (body/nav), both via Google Fonts
- Cards flip background against their section (white cards on sand sections,
  sand cards on white sections) — intentional, keep it that way when editing

## Before you deploy

- Email is already set to `contactydpa@gmail.com` throughout.
- "Oakland School for the Arts" is intentionally not named anywhere on this
  site — only "Oakland Unified School District" is mentioned. Add a specific
  school once that partnership is formally confirmed.

## Local preview

Just open `index.html` in a browser — no install needed.

## Deploying (GitHub + Vercel)

1. Create a new GitHub repository and upload all files in this folder
   (keep the `css/` and `js/` folder structure intact).
2. Go to vercel.com → sign in with GitHub → Add New Project → import the repo.
3. Leave build settings as default (it's a static site) → Deploy.
4. To connect your GoDaddy domain: Vercel project → Settings → Domains → add
   your domain → copy the DNS records shown → add them in GoDaddy's DNS
   management for that domain.

## File structure

```
ydpa-website/
  index.html
  about.html
  initiatives.html
  contact.html
  css/style.css
  js/main.js
  README.md
```
