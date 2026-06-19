# Curriculum OS — landing page

Static landing page for Curriculum OS (the curriculum operating system that learns your way of teaching).
No build step — plain HTML/CSS/JS. Hosted on **Netlify**, code on **GitHub**, DNS on **Squarespace**.

## Files
- `index.html` — the landing page (all CSS/JS inline)
- `thanks.html` — post-application confirmation page (form redirects here)
- `logo.svg` — brand mark (ring + book + spark)
- `favicon.svg` — favicon
- `netlify.toml` — Netlify config (publish root, security headers, asset caching)
- `robots.txt`
- `notes/` — internal working docs (grounding, logo concepts) — not part of the live site

## Lead capture
The "Apply for a place" form uses **Netlify Forms** (`name="founding-access"`, `data-netlify="true"`).
Submissions appear in **Netlify → Forms**. On success it redirects to `/thanks.html`.
Set up notifications in Netlify → Forms → Settings to email each application to michael@bobldobl.com.

---

## 1 — Push to GitHub (GitHub CLI)

From this folder:

```bash
git add -A
git commit -m "Curriculum OS landing page"
# create a NEW public repo and push (you'll be prompted to auth on first use)
gh repo create curriculum-os --public --source=. --remote=origin --push
```

(Repo already initialised with a first commit. If you'd rather use the existing
`bobldobl-landing-page` repo, set the remote to that instead and push to a new branch.)

## 2 — Deploy on Netlify

1. Netlify → **Add new site → Import an existing project → GitHub** → pick `curriculum-os`.
2. Build command: **(leave blank)**. Publish directory: **`.`** (root). Deploy.
3. You'll get a temporary URL like `curriculum-os.netlify.app` — note the exact site name.

## 3 — Custom domain + Squarespace DNS

Decide the domain first (e.g. `curriculum-os.com`, or a subdomain of bobldobl.com).
In **Netlify → Domain management → Add a domain**, enter it. Then in **Squarespace → your domain → DNS settings** add:

**Apex / root (`@`)** — one of:
- Preferred (if available): **ALIAS / ANAME** → `apex-loadbalancer.netlify.com`
- Fallback: **A record** → `75.2.60.5`

**www** — **CNAME** → `YOUR-SITE-NAME.netlify.app` (the exact name from step 2)

Remove any old/conflicting A or CNAME records for `@` and `www` that point at the current site.
Enable **HTTPS** in Netlify once DNS verifies (it provisions a free Let's Encrypt cert). DNS can take up to ~24h to propagate.

> Squarespace's built-in DNS doesn't support ALIAS for external targets, so for an apex on Squarespace use the **A record `75.2.60.5`** + **www CNAME**. Then set your preferred domain (apex or www) in Netlify and let it redirect the other.
