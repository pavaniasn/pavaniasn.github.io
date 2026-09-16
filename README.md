# pavaniasn.github.io

Personal site. Plain HTML pages, plus a Jekyll collection for the writing section.

## Adding a new piece to Mananam

1. Create one new file in `_mananam/`, named `YYYY-MM-DD-short-name.md`
   (the date prefix just keeps the folder in order).

2. Start it with this block, then write the piece underneath in plain text:

```markdown
---
title: "Your Title Here"
slug: your-title-here
summary: >-
  One or two sentences. This is what shows on the Mananam index page
  and in Google results — so make it inviting, not a summary.
date: 2026-08-15
---

Your first paragraph.

Your second paragraph. Leave a blank line between paragraphs.

Use *asterisks* around book, film, or article titles to italicise them.
```

3. Commit and push. GitHub rebuilds the site in a minute or two.

That's it — the piece appears at the top of `writing.html` automatically, and gets
its own page at `/mananam/your-title-here/`. Nothing else needs editing.

**The `slug` becomes the web address, so don't change it after you've shared a link.**

## Layout of the repo

| Path | What it is |
|---|---|
| `_mananam/` | One file per piece of writing. This is the only folder you need for new posts. |
| `_layouts/mananam.html` | The frame around a single piece — nav, title, footer. |
| `writing.html` | The Mananam index. Lists everything in `_mananam/` automatically. |
| `style.css` | All styling for the whole site. |
| `index.html`, `research.html`, `portfolio.html`, `teaching.html`, `contact.html`, `appointments.html` | Ordinary HTML pages, edited by hand. |
| `_config.yml` | Site settings. Rarely needs touching. |

Note: the navigation menu is repeated at the top of each HTML page. If you add or
rename a menu item, it has to be changed in each of those files.
