# Personal website

A plain Jekyll site that GitHub Pages builds for you. No themes, no JavaScript, one CSS file.

## Put it online (one time)

1. Create a public GitHub repo named exactly `<your-username>.github.io`.
2. Upload everything in this folder to it (drag and drop on the repo page works, or `git push`).
3. Go to **Settings → Pages**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute the site is live at `https://<your-username>.github.io`.

## Where to edit what

| To change…                         | Edit this file              |
|------------------------------------|-----------------------------|
| Name, email, profile links, nav    | `_config.yml`               |
| Home page bio                      | `index.md`                  |
| News lines on Home                 | `_data/news.yml`            |
| Papers and preprints               | `_data/publications.yml`    |
| Research page text                 | `research.md`               |
| Projects list                      | `_data/projects.yml`        |
| CV page / CV PDF                   | `cv.md` / `assets/cv.pdf`   |
| Misc page                          | `misc.md`                   |
| Colors, fonts, spacing             | `assets/css/style.css`      |
| Header, nav, footer HTML           | `_layouts/default.html`     |

Easiest way to edit: open the repo on github.com and press `.` to get an editor in the browser.
Commit, and the site rebuilds in about a minute.

## Common tasks

**Add a paper:** copy an entry in `_data/publications.yml`, put the PDF in `assets/papers/`.

**Write a blog post:** add `_posts/YYYY-MM-DD-short-title.md` with this at the top:

```
---
layout: post
title: "Your title"
tags: [fair division]
math: true        # only if the post has LaTeX
---
```

**Add a page:** create `newpage.md` with `layout: default` and `title:` front matter, then add it to `nav` in `_config.yml`.

**Add your photo:** save a square photo as `assets/img/photo.jpg` and set `photo: /assets/img/photo.jpg` in `_config.yml`.

**Change colors:** the light theme is the first block in `assets/css/style.css`; the dark theme is the two blocks right after it (keep those two identical). The Light/Dark button in the nav remembers each visitor's choice.

## Before going live

Everything marked with `[brackets]`, `your-username`, `XXXX`, or a "sample" comment is a placeholder.
Search for those and replace them. Also add `assets/cv.pdf`.

## Preview on your own computer (optional)

```
gem install jekyll
jekyll serve
```

Then open http://localhost:4000.
