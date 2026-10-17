# Afferium Blog

A Markdown blog using the visual language of afferium.com: the original textured background, coral accents, serif headings, and warm text. Article lists and article pages are built automatically from Markdown. No HTML editing is needed to publish an essay.

## Publish an essay

1. Open `templates/essay.md` in GitHub and copy its contents.
2. In `essays/`, choose **Add file → Create new file**. Name it `YYYY-MM-DD-short-title.md`, for example `2026-10-17-my-first-essay.md`.
3. Paste the template. Change the title, date, summary, and tags, then replace the sample text with your essay.
4. Keep `published: false` while working. When ready, change it to `published: true` and commit to `main`.
5. **Actions → Publish blog** shows the build and deployment. A successful run updates both the essay and its entry on the homepage.

The small metadata block at the top looks like this:

```yaml
---
title: "Your essay title"
date: 2026-10-17
summary: "A short introduction shown beneath the title on the homepage."
tags: [Ideas, Technology]
published: false
---
```

- Use quotation marks around titles and summaries. Use `true` or `false` without quotation marks.
- Name files with lowercase words separated by hyphens. The filename after the date becomes the essay's stable address.
- A file in `drafts/` is always excluded from live output. Files in `essays/` with `published: false` are also excluded.
- Drafts in a **public GitHub repository are still visible as source files**. Keep private or sensitive drafts outside the public repository until ready.
- Future-dated essays are excluded until a build runs on or after their date in America/New_York. This setup publishes on commits; it does not schedule future posts.
- Update an essay by editing its Markdown and committing again. Preserve its filename to preserve its address.
- Make headings with `##`, italics with `*text*`, bold with `**text**`, links with `[label](https://...)`, and quotations with `>`.
- Footnotes use `[^note]` in the essay and `[^note]: Source information` below it. The template includes an example.
- To add a local image, put it in `assets/` and use `![Description](../../assets/filename.jpg)` in the essay.

## One-time GitHub Pages setup

This folder is a standalone project. Copy its **contents, including `.github/`**, into the root of a new repository such as `Afferium/blog`, on its `main` branch. Do not set this as the publishing source of the existing afferium.com repository: each repository has one Pages site.

1. In the blog repository, open **Settings → Pages** and choose **GitHub Actions** under Build and deployment.
2. In **Custom domain**, enter `afferium.blog` and save it.
3. In the domain's DNS provider, point its apex (`@`) at GitHub Pages using the four A records below. Add the `www` CNAME if you want that address too. Remove conflicting apex forwarding or parking records.

| Type | Host | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | Afferium.github.io |

4. Run **Actions → Publish blog → Run workflow**, or commit to `main`.
5. After DNS verifies and the certificate is ready, enable **Enforce HTTPS**.

The workflow uses GitHub's normal Pages authentication. No personal access token needs to be added. If the organization has an Actions approval or restriction, its administrator must allow the listed official GitHub actions.

Official setup references:

- https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

## Preview locally

With Python 3.12 or later:

```sh
python -m pip install -r requirements.txt
python build.py --preview
python -m http.server 8000 --directory preview
```

Open `http://localhost:8000`. Preview pages include drafts and display a preview notice. `drafts/essay-layout-preview.md` is sample text for reviewing the article typography, not an actual essay. It never enters the live build.

For the actual publishing build, run `python build.py`. The generated site is in `_site/`; it contains only published, non-future essays. GitHub Actions builds this production version. Templates, drafts, scripts, and source Markdown are not copied into the deployed website.

## Files

- `site.json` — site name, description, domain, and timezone.
- `essays/` — Markdown essays.
- `drafts/` — optional public-source drafts and layout sample, excluded from live output.
- `templates/essay.md` — reusable essay template.
- `layouts/` and `assets/blog.css` — homepage, article layout, and visual styles.
- `build.py` — Markdown conversion, metadata validation, homepage list, and production/preview separation.
- `.github/workflows/pages.yml` — rebuild and publish automatically on commits to `main`.

Public source does not grant reuse rights to the essays or artwork. Copyright remains with their owner.
