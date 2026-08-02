# tysonchae.github.io

A minimal Jekyll blog with full-text search powered by [Pagefind](https://pagefind.app).

## Write a new post

Add a markdown file to `_posts/` named `YYYY-MM-DD-title.md`:

```markdown
---
title: "Post title"
tags: [team, culture]
---

Your writing here.
```

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000`. Note: search won't work locally unless you
also run Pagefind against the built `_site/` folder — it's wired up
automatically on every push via GitHub Actions (see
`.github/workflows/deploy.yml`), so search works on the live site.

## Enable GitHub Pages (one-time setup)

In the repo: **Settings → Pages → Build and deployment → Source →
GitHub Actions**. After that, every push to `main` builds and deploys
automatically.

## Structure

```
_posts/     Blog posts (this is what you'll touch most)
_layouts/   Page templates (default, post)
_includes/  Header, footer, head
assets/css/ All styling — one file, style.css
about.md    About page
search.html Full-text search page (Pagefind)
```
