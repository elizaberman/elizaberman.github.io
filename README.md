# elizaberman.github.io

Personal site, built with plain Jekyll. Edit files on github.com (pencil icon) or locally. Every push to `main` rebuilds and publishes the site in about a minute.

## What to edit

| To change… | Edit |
| --- | --- |
| Bio (next to the photo) | `_pages/about.md`, below the `---` line |
| Research section | `_pages/about.md`, the `research:` block at the top |
| Publications | `_data/publications.yml` (template at the top of the file) |
| Name, title line, email, link buttons | `_config.yml` |
| Photo | replace `assets/img/prof_pic.jpg` (same file name) |
| Colors, fonts, spacing | `assets/css/style.css` |
| Page structure | `_layouts/` (`default.html` = top bar + footer, `about.html` = homepage, `page.html` = other pages) |

Bio and research text are Markdown: `**bold**`, `*italics*`, `[link text](https://...)`, and a blank line between paragraphs.

Publications appear in the order they're listed, so add new ones at the top. Your name is bolded in author lists automatically.

## Adding a page

Create a file in `_pages/`, e.g. `_pages/teaching.md`:

```markdown
---
layout: page
title: Teaching
permalink: /teaching/
nav: true        # show it in the top bar
nav_order: 1     # position in the top bar (lower = further left)
---

Page content in Markdown.
```

## Preview locally (optional)

```sh
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
