# Cyber Writeup Template

A ready-made Jekyll site for GitHub Pages. You add one markdown file with your writeup, and GitHub turns it into a styled website.

## Steps

1. **Click "Use this template" → "Create a new repository."**
   - Name it exactly **cyber-research**.
   - Set it to **Public**.
2. **Edit `_config.yml`** (click the file, then the pencil icon). Change the title, description, and author. You can also pick your look: the file lists four themes (hacker, midnight, cayman, slate). Keep one without a `#` in front of it. Then click **Commit changes**.
3. **Add your writeup.** Open the `_posts` folder, then **Add file → Create new file**.
   - The file name must look like `2026-10-07-my-topic.md`: today's date, then a short name with dashes, ending in `.md`.
   - Paste in the post from your AI (see the prompt below), then **Commit changes**.
4. **Delete the sample post:** open `_posts/2026-10-07-sample-post.md`, click the trash icon, and commit.
5. **Turn on Pages:** **Settings → Pages → Deploy from a branch → `main` / `(root)` → Save.**
6. **Wait 1 to 2 minutes**, then refresh the Pages settings. Your link appears at the top: `https://yourusername.github.io/cyber-research/`.

## Prompt for your AI

```
Turn the writeup below into ONE Jekyll post. Output only the file contents.

Start with this front matter, exactly:
---
layout: default
title: "YOUR TITLE"
date: YYYY-MM-DD
tags: [cybersecurity]
---

Use today's date with no time. Right after the front matter, start the body with a "# YOUR TITLE" heading (the theme does not show the title by itself). Then write the rest in markdown with ## headings, and end with a "## Sources" section that links every source I used. Put any title that contains a colon inside the quotes.

Also tell me what to name the file (YYYY-MM-DD-short-title.md).

WRITEUP:
[paste your NotebookLM writeup here]
```

## If something goes wrong

- **"There isn't a GitHub Pages site here" or a 404:** wait two more minutes. Check that the repo is **Public** and that Settings → Pages shows a link.
- **The site works but looks plain, with no styling:** your repo isn't named exactly `cyber-research`. Open `_config.yml` and make sure the `baseurl` line matches your repo name, with a slash in front.
- **My post doesn't show up:**
  - Is it inside the `_posts` folder?
  - Is the file name `YYYY-MM-DD-title.md`?
  - Is the date today or earlier? Future dates are hidden.
  - Does the file start with `---` on the first line, and have another `---` after the front matter?
- **The look didn't change:** make sure exactly one `theme:` line has no `#` in front of it, then wait a minute and hard-refresh the page.
- **Red X on the **Actions** tab:** click the failed run to read the error. It's usually a typo in the front matter, like a missing quote.
- **Still stuck:** copy the error and your file into your AI and ask what's wrong.
