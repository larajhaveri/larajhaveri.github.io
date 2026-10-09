# Personal Portfolio

A static Markdown portfolio built with Jekyll for GitHub Pages. Keep all site source files at the repository root; publishing is configured for `main` / (root).

## Useful commands

- `bundle exec jekyll serve` — preview locally at `http://127.0.0.1:4000`
- `bundle exec jekyll build` — build to the ignored `_site/` directory

## Content and design

- Markdown pages with YAML front matter are the source of page content.
- Shared HTML lives in `_layouts/` and `_includes/`; styling and illustrations live in `assets/`.
- Keep supplied career facts verbatim in meaning. Do not invent employers, dates, achievements, projects, or metrics. Replace visible placeholders only with details the user provides.
- The public contact link is `mailto:larajhaveri@berkeley.edu`.
- Use a light, clean, warm, human, bubbly, and fun feel while keeping the layout simple, single-column, responsive, and accessible.
- Do not fetch the user's personal information from URLs; use pasted copy or an uploaded résumé.
- Do not add a Node/React/Vite app, package.json, backend, database, blog, CMS, contact-form backend, animation framework, or third-party trackers.
- Target Lighthouse scores of at least 90 for Performance, Accessibility, Best Practices, and SEO.

## Publishing

GitHub Pages builds the site from the `main` branch and repository root. `url` is `https://larajhaveri.github.io` and `baseurl` is empty.
