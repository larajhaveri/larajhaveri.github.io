# Portfolio site plan

## Goal

Build a responsive personal portfolio for `larajhaveri.github.io`, published by GitHub Pages from the `main` branch and repository root. Keep the project itself a static Jekyll site; do not add an app framework, server, database, or tracking.

## Pages and content

- **Home:** A concise introduction and the user's stated interest in consumer-tech product strategy and product management.
- **About:** The supplied MBA and career narrative, without adding unprovided facts.
- **Work Experience:** BlueRobins, Delivery Hero, and the unnamed Singapore HR-tech startup, using only the details supplied. Do not invent dates, startup name, metrics, projects, or results.
- **Contact:** A public `mailto:larajhaveri@berkeley.edu` link and a clear note that it opens visitors' email app.

Use visible placeholders for the user's name, dates, LinkedIn URL, and any photos or project links not supplied. Clickable visual elements must not imply an unprovided project or achievement.

## Visual direction

Use a light, clean, warm, human, bubbly, and fun feel, informed by the user's references: clickable imagery, sports/outdoors, medal details, and playful bubble effects. Keep the layout simple and single-column, with responsive navigation, accessible contrast, semantic HTML, and a shared footer.

## Jekyll and publishing

Keep `index.md`, `_config.yml`, `_layouts/`, `_includes/`, styles, favicon, sitemap support, SEO metadata, and README directly in the repository root. Use Markdown pages with YAML front matter and reusable layouts/includes. Set `url` to `https://larajhaveri.github.io` and `baseurl` to `""`; use Jekyll URL filters for links. Document local preview, content updates, and Lighthouse checks in README.

## Important scope change and assumptions

To make the root publishable as only the requested site, implementation will replace the generated pnpm workspace scaffold and remove its API server, mockup canvas, libraries, and scripts. No supplied personal photos, work samples, dates, full name, or LinkedIn profile URL are assumed to exist; those remain labeled placeholders until provided. GitHub Pages is assumed to publish `main` / (root).
