# Your Articles — Free Website (GitHub Pages)

This folder is a complete website you can host for free with **GitHub Pages**. It’s built with Jekyll + the Minima theme and includes custom fonts/colors and a starter article.

---

## Step-by-step: Put it online (free)

**A. Create the repository**
1. Go to https://github.com and sign in (or create an account).
2. Click **New** repository.
3. Name it anything (e.g. `my-articles`) and choose **Public**.
4. Click **Create repository**.

**B. Upload the site files**
1. On your new repo page, click **Add file → Upload files**.
2. Drag all files from this folder into the GitHub upload page.
3. Scroll down and click **Commit changes**.

**C. Turn on GitHub Pages**
1. Go to **Settings → Pages** (left sidebar).
2. Under **Source**, choose **Deploy from a branch**.
3. Under **Branch**, pick `main` (or `master`) and `/ (root)`.
4. Click **Save**.
5. In about a minute, your site will be live at:  
   `https://<your-username>.github.io/<your-repo>/`

> **Tip:** If you name the repo exactly `your-username.github.io`, your site will live at `https://your-username.github.io/` and you should keep `baseurl: ""` in `_config.yml` (already set).

---

## Customize the look & feel

- **Title & description:** Edit `_config.yml`.
- **Logo:** Replace `assets/img/logo.svg` with your own file (same name to keep header working).
- **Colors & fonts:** Adjust `assets/css/style.scss` (accent color is `--accent`, font is Inter).
- **About page:** Edit `about.md`.

---

## Add a new article

1. In the repo, open the `_posts/` folder → **Add file → Create new file**.
2. Name it `YYYY-MM-DD-your-title.md` (e.g., `2025-01-12-my-first-post.md`).
3. Paste this at the top:

```yaml
---
layout: post
title: "My Article Title"
date: 2025-01-12 10:00:00 +0000
categories: notes
tags: [tag1, tag2]
---
```

4. Write your content in **Markdown** below that block.
5. Click **Commit changes** — it will publish automatically.

---

## Optional: Custom domain

1. Buy a domain from a registrar (e.g., Namecheap).
2. In your repo, click **Settings → Pages** and add your domain under **Custom domain**.
3. At your registrar, create a CNAME record pointing to `your-username.github.io`.
4. Wait for DNS to propagate.

---

## Local preview (optional, advanced)

If you want to preview locally:

```bash
# Requires Ruby + Bundler + Jekyll installed
bundle init
bundle add jekyll
bundle exec jekyll serve
```

You can skip this because GitHub Pages builds for you on the server.

---

**You’re done.** Publish articles whenever you like — just add a file to `_posts/`.
