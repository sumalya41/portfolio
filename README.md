# Sumalya Bhattacharya — portfolio site

A static site (plain HTML, no build step), ready for Vercel.

```
index.html     the page
resume.pdf     your CV, linked from the "Résumé" button
favicon.svg    browser-tab icon
vercel.json    clean URLs and basic security headers
```

## Deploy on Vercel (option A: GitHub, recommended)

1. Create a new GitHub repository, e.g. `sumalya41/portfolio`, and upload these four files to its root.
2. Go to vercel.com → **Add New… → Project** → import that repository.
3. Framework preset: **Other**. Leave Build Command and Output Directory empty. Click **Deploy**.
4. Your site is live at `https://<project-name>.vercel.app`. Every push to the repo redeploys it.

## Deploy on Vercel (option B: command line)

```bash
npm i -g vercel
cd portfolio
vercel          # first run: log in and accept the defaults
vercel --prod   # publish to your production URL
```

## Custom domain (optional)

In the Vercel project: **Settings → Domains → Add**, then follow the DNS instructions.

## Editing

- All text lives in `index.html`. Each project is one `<article class="proj">` block; copy one to add a project.
- To update your CV, replace `resume.pdf` with a file of the same name.
- Colours and fonts are defined once at the top of the `<style>` block (`:root`).
