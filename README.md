# Thinking Through — Danial's blog

A minimal, fully-owned static blog. Posts are plain Markdown files; GitHub builds and publishes the site automatically.

## How to publish a post (the everyday workflow)

1. Go to your repository on github.com → `posts` folder → **Add file → Create new file**.
2. Name it `YYYY-MM-DD-short-title.md` (e.g. `2026-08-01-on-observation.md`).
3. Start the file with:

   ```
   ---
   title: On observation
   category: Pedagogy
   summary: One line that appears on the home page.
   ---
   ```

   Then write in Markdown below it. `category` and `summary` are optional.
4. Click **Commit changes**. The site rebuilds and updates itself in about a minute.

You can also edit any existing post the same way — open the file on github.com and click the pencil icon.

## Change the blog title, tagline, or author

Edit `_data/site.json`.

## Edit the About page

Edit `about.md`.

## One-time setup (already done if you are reading this on GitHub)

1. Create a repository named `YOUR-USERNAME.github.io` (public).
2. Upload all files in this folder to it, keeping the folder structure.
3. In the repository: **Settings → Pages → Source → GitHub Actions**.
4. Wait for the Action to finish (green tick in the **Actions** tab). Site is live at `https://YOUR-USERNAME.github.io`.

## Optional: run locally

Requires Node.js. `npm install`, then `npm run serve` and open http://localhost:8080.
