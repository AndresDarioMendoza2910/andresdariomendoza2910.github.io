# Andrés Mendoza — Portfolio

A static portfolio site. No build step, no backend, no dependencies — just HTML + CSS + a little vanilla JS. Hosts free on GitHub Pages.

## Files
```
index.html                         landing page (hero, projects grid, about, contact)
projects/staffing-automation.html  the first case study
assets/style.css                   all styling (dark developer theme)
```

## Before you publish — 2 edits
1. **LinkedIn link.** Search the project for `LINKEDIN_URL_HERE` (it appears in the footer of both pages) and replace it with your LinkedIn URL. If you don't want LinkedIn, delete that `<a>` line.
2. That's it. Everything else (name, email, GitHub, content) is already filled in.

## Deploy to GitHub Pages (free, ~5 minutes)

**Option A — through the GitHub website (no git needed):**
1. Go to github.com → **New repository**. Name it e.g. `portfolio` (or `andresdariomendoza2910.github.io` to get a cleaner URL — see note below). Make it **Public**. Create.
2. On the new repo page, click **uploading an existing file**.
3. Drag in `index.html`, the `assets` folder, and the `projects` folder (keep the folder structure). Commit.
4. Go to the repo's **Settings → Pages**.
5. Under **Build and deployment → Source**, choose **Deploy from a branch**. Branch: **main**, folder: **/ (root)**. Save.
6. Wait ~1 minute. Your site is live at:
   - `https://<your-username>.github.io/portfolio/`  (if repo named `portfolio`)
   - `https://<your-username>.github.io/`  (if repo named `<your-username>.github.io`)

**Option B — with git (if you use it):**
```bash
git init
git add .
git commit -m "portfolio"
git branch -M main
git remote add origin https://github.com/<you>/portfolio.git
git push -u origin main
# then enable Pages in Settings → Pages (same as step 4–5 above)
```

### Note on the URL
Naming the repo `<your-username>.github.io` gives you the clean root URL (`https://andresdariomendoza2910.github.io/`) with no `/portfolio/` suffix. Any other repo name puts the site under that path. Both are free and permanent.

## Custom domain (optional, later)
GitHub Pages supports a custom domain for free (you only pay for the domain itself, ~$10/yr, if you ever want one). Settings → Pages → Custom domain.

## Adding more projects later
Copy `projects/staffing-automation.html` to a new file, edit the content, and add a matching `<a class="card">` block to the projects grid in `index.html`. The "Coming soon" card is a placeholder you can replace.
