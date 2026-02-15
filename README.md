# Shining Venus

Shining Venus is a personal website and blog built with **Jekyll** and hosted via **GitHub Pages**. It serves as a quiet, long-form space for project notes, creative writing, and personal reflections.

## About the app

This repository powers a static website with:

- A homepage that lists blog posts
- Individual post pages with metadata (date, categories, tags)
- An About page for profile/contact information
- Reusable layouts and includes for consistent styling and metadata
- Sass-based styling for easy theme customization

Because the site is static, deployment is simple and fast: push changes to GitHub and GitHub Pages rebuilds the site.

## Tech stack

- **Jekyll** (static site generator)
- **GitHub Pages** (hosting/build)
- **Liquid** templates (layouts/includes)
- **Sass** for styles

## Repository structure

- `_config.yml` — site configuration (name, description, links, base URL)
- `_posts/` — blog posts (Markdown)
- `_layouts/` — page/post/default layouts
- `_includes/` — shared partials (meta tags, analytics, icons)
- `_sass/` and `style.scss` — styling
- `about.md` — About page content
- `index.html` — homepage post listing

## Running locally

1. Install dependencies:
   ```bash
   gem install bundler jekyll
   bundle install
   ```
2. Start the dev server:
   ```bash
   bundle exec jekyll serve
   ```
3. Open:
   ```text
   http://127.0.0.1:4000
   ```

## Writing content

### Create a new post

Add a Markdown file in `_posts/` using this filename format:

```text
YYYY-MM-DD-title.md
```

Use front matter like:

```yaml
---
layout: post
title: "Post Title"
date: 2026-02-14
categories: blog
tags: [tag1, tag2]
---
```

### Update site information

Edit `_config.yml` to change:

- Site name and description
- Avatar
- Footer/social links
- Analytics or comments settings

## Deployment

This site is intended for GitHub Pages deployment:

1. Push to the default branch.
2. GitHub Pages builds and publishes automatically.
3. Visit your configured GitHub Pages URL.

## License

See [`LICENSE`](LICENSE) for project licensing information.
