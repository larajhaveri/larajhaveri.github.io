# Personal portfolio

A static Jekyll site for `larajhaveri.github.io`. Page content is Markdown with YAML front matter; shared structure is in `_layouts/` and `_includes/`, and the site's styling and images are in `assets/`.

## Update the site

- Edit `index.md`, `about.md`, `work-experience.md`, or `contact.md` to update page content.
- Keep facts accurate. Replace bracketed placeholders only with details you want made public.
- Update navigation in `_data/navigation.yml`.
- Adjust colors, spacing, and responsive styling in `assets/css/style.css`.
- Replace the illustration placeholders in `assets/images/` with personal images only if you choose to provide them; update each image's alternative text at the same time.
- Update the public email address in `contact.md` and `_includes/footer.html` if it changes.

## Preview locally

Install Ruby and Bundler, then from the repository root run:

```sh
bundle install
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`. Jekyll reloads the generated site as you edit files. To build once without serving:

```sh
bundle exec jekyll build
```

The generated `_site/` directory is local output and is ignored by Git.

## Publish with GitHub Pages

This is a GitHub user site for `larajhaveri.github.io`:

1. Use a repository named `larajhaveri.github.io`.
2. Push the site files to the `main` branch.
3. In the repository's Pages settings, choose **Deploy from a branch**, then select `main` and `/(root)`.
4. GitHub Pages runs Jekyll for the source directly; no separate build or deploy command is needed.

`_config.yml` sets `url` to `https://larajhaveri.github.io` and leaves `baseurl` empty. Internal links and asset paths use Jekyll's `relative_url` filter.

## Run Lighthouse

For a repeatable manual check, start the local preview, open it in Chrome, then choose **DevTools → Lighthouse**. Run both Desktop and Mobile reports and check Performance, Accessibility, Best Practices, and SEO. The layout is designed to remain readable at 375px and 1280px. No trackers, external fonts, images, or runtime JavaScript are required.

## Assumptions and placeholders

- The user's full display name, work dates, startup name, LinkedIn URL, personal photos, and work samples were not supplied and are visibly marked as placeholders.
- The contact email is intentionally public and opens visitors' email app.
- The two local illustrations are labeled placeholders; the medal is decorative and does not indicate an award.

## Technical choices

- GitHub Pages-compatible Jekyll with reusable layouts and includes.
- GitHub Pages SEO and sitemap plugins, with a local `github-pages` Gemfile for preview parity.
- Plain semantic HTML, CSS, local SVG illustrations, and no JavaScript, backend, database, or third-party trackers.
