---
layout: post
title: "Deploying a Personal Homepage on GitHub Pages: A Practical Guide"
date: 2026-08-06
tags: [Jekyll, GitHub Pages, Web]
image: /assets/img/blog-thumb.svg
excerpt: "How I set up my academic homepage with the Minimal Light Jekyll theme and GitHub Pages, including proxy and deployment tips."
---

Building a personal academic homepage is easier than it looks — if you know a few tricks. This post documents my experience deploying this site with the **Minimal Light** Jekyll theme on **GitHub Pages**.

## Why GitHub Pages?

- **Free** hosting with automatic HTTPS
- Native **Jekyll** support — no build server needed
- Version control with Git for free

## Steps I Followed

### 1. Repository naming matters

For a user site, the repository must be named exactly `username.github.io` (e.g., `simaqie.github.io`). Any other name produces a project site at a sub-path.

### 2. Theme setup

Use a `remote_theme` in `_config.yml`:

```yaml
remote_theme: yaoyao-liu/minimal-light
```

GitHub Pages resolves the remote theme automatically during build.

### 3. Push with a proxy

If your network has trouble reaching GitHub directly, configure Git to go through a local proxy:

```bash
git -c http.proxy=http://127.0.0.1:7890 push
```

For large initial pushes, also raise the buffer:

```bash
git -c http.postBuffer=524288000 push
```

### 4. Customize content

- Sidebar info lives in `_config.yml`
- Page content lives in `index.md`
- Blog posts go into `_posts/` with `YYYY-MM-DD-title.md` naming

## Key Takeaways

1. GitHub Pages auto-builds Jekyll sites — push and wait 1–2 minutes
2. Check the build status at `https://github.com/USERNAME/USERNAME.github.io/actions`
3. Keep `_config.yml` small; local overrides (like `_layouts/`) take precedence over the remote theme

Happy building!
