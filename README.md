# CRC Earth Analytics Blog

Source for [crceanalytics.com](https://www.crceanalytics.com), built with [Hugo](https://gohugo.io) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

## Writing a new post

Create a markdown file in `content/posts/`:

```bash
hugo new content posts/my-post-title.md
```

Or create the file manually with this frontmatter:

```markdown
---
title: My Post Title
date: 2026-06-26
categories: ["hydrology"]
tags: ["tag1", "tag2"]
description: Optional short summary shown in post listings.
---

Post content here.
```

Images go in `static/images/` and are referenced as `/images/filename.png`.

## Local preview

```bash
hugo server
```

Then open [http://localhost:1313](http://localhost:1313). The server live-reloads on file changes.

## Deployment

Push to `main` — GitHub Actions builds the site and deploys to GitHub Pages automatically.

```bash
git add content/posts/my-post-title.md
git commit -m "Add post: my post title"
git push
```

## One-time setup (if cloning fresh)

```bash
# Clone with the PaperMod submodule
git clone --recurse-submodules https://github.com/chrisrycx/chrisrycx.github.io.git

# Install Hugo extended v0.147.0+
wget https://github.com/gohugoio/hugo/releases/download/v0.147.0/hugo_extended_0.147.0_linux-amd64.deb
sudo dpkg -i hugo_extended_0.147.0_linux-amd64.deb
```

GitHub Pages must have Source set to **GitHub Actions** in the repo Settings → Pages.
