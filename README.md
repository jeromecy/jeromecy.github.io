# zcao.space — Personal Website & Blog

Personal website of Dr. Zhanglong Cao — Lecturer in Statistics (EECMS, Curtin University). Research in agricultural statistics, Bayesian methods, and data analytics.

Live at **<https://www.zcao.space>**. Built with [Quarto](https://quarto.org).

## Structure

```
MyBlog/
├── _quarto.yml      # Site configuration (navbar, theme, resources)
├── index.qmd        # Homepage (hero, featured tools, latest posts)
├── posts/           # Blog posts (.qmd), listed on posts.qmd with categories + RSS
├── about.qmd        # About page
├── cv.qmd           # Curriculum Vitae
├── projects.qmd     # Research projects & applications
├── contact.qmd      # Contact form and details
├── custom.scss      # Theme customisation on top of the cosmo Bootstrap theme
├── assets/, PDF/    # Static resources (images, slide decks, PDFs)
└── .github/workflows/publish.yml   # CI: render + publish to gh-pages
```

## Local development

```sh
quarto preview     # live-reloading local server
quarto render      # build to _site/
```

No Ruby/Jekyll required — the site migrated from Jekyll to Quarto in July 2026.
Old Jekyll URLs (e.g. `/posts/<title>/`, `/cv/`, `/privacy/`) are preserved via
Quarto `aliases` redirects.

## Writing a post

Create `posts/YYYY-MM-DD-slug.qmd`:

```yaml
---
title: "Post Title"
date: 2026-07-13
categories: [Statistics, R]
description: "One-line summary shown in listings."
---
```

Markdown, LaTeX math, and executable R/Python code cells are all supported.

## Deployment

Pushing to `master` triggers the GitHub Action, which renders the site and
publishes it to the `gh-pages` branch. GitHub Pages must be configured to serve
from `gh-pages` (root). The custom domain is set via the `CNAME` resource.

## Links

- **Live Site**: [www.zcao.space](https://www.zcao.space)
- **GitHub**: [jeromecy](https://github.com/jeromecy)
- **LinkedIn**: [zhanglong-cao](https://linkedin.com/in/zhanglong-cao-72208487)

## License

MIT — see [LICENSE](LICENSE).
