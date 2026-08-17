# Youth Drug Protection Alliance — website

A 5-page static site: `index.html` (home), `about.html` (mission), `programs.html`,
`partners.html` (get involved), and `contact.html`. No build step, no framework —
just plain HTML, CSS, and a small JS file, so it deploys on Vercel with zero
configuration and is easy to hand-edit later.

## Before you deploy — things to personalize

- **Email address**: replace `hello@youthdpa.org` (appears in `contact.html`,
  `index.html`, `about.html`, `programs.html`, `partners.html` footers) with your
  real email once you have one.
- **School name**: the site currently says "a partner high school in Oakland"
  rather than naming Oakland School for the Arts directly. Swap in the real name
  once OSA has formally agreed to be publicly associated with the program —
  worth confirming with your contact there first.
- **Partner organizations**: the "Get involved" page intentionally doesn't name
  Punks with Lunch, HEPPAC, Fentcheck, etc. as confirmed partners yet, since
  outreach is still in progress. Add them once a relationship is actually
  confirmed — listing an org before they've agreed can create problems.
- **Domain**: replace any placeholder references once your GoDaddy domain is
  connected (see deployment steps below).

## Local preview

No install needed. Just open `index.html` in a browser, or, if you have Python
installed, run this from the project folder for a local server:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploying (GitHub + Vercel + GoDaddy domain)

See the full step-by-step walkthrough in the chat where this was generated.
Short version:

1. Push this folder to a new GitHub repository.
2. Import that repository into Vercel (vercel.com → Add New Project).
3. Vercel deploys automatically — no build settings needed for a static site.
4. In Vercel, go to your project → Settings → Domains, and add your GoDaddy
   domain.
5. In GoDaddy's DNS settings, add the DNS records Vercel gives you.
6. Wait for DNS to propagate (a few minutes to ~48 hours), then your domain
   points at the live site.

## File structure

```
ydpa-website/
  index.html
  about.html
  programs.html
  partners.html
  contact.html
  css/style.css
  js/main.js
  README.md
```
