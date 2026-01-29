# Repository Guidelines

## Project Structure & Module Organization
- `_layouts/` and `_includes/` contain Jekyll templates and shared partials.
- `index.md` and the `en/` and `kr/` directories hold page content in Markdown/HTML.
- `_data/` stores YAML data files used by templates (e.g., organizers, staff, index content).
- `assets/` contains compiled site assets: `assets/sass/` for Sass sources, `assets/css/` for CSS, `assets/js/` for scripts, and `assets/webfonts/`.
- `images/` and `static_data/` hold media and downloadable resources.
- `_site/` is the generated output from Jekyll; do not edit it directly.

## Build, Test, and Development Commands
- `jekyll serve`: Build the site and run a local dev server (default at http://127.0.0.1:4000).
- `jekyll build`: Generate the static site into `_site/` for deployment.

## Coding Style & Naming Conventions
- Follow existing formatting in Markdown/HTML files; keep front matter keys in YAML format at the top of pages.
- Sass uses tabs for indentation in existing files; match the current style when editing `assets/sass/`.
- Prefer descriptive page filenames and section names (e.g., `en/registration.md`, `kr/rules.md`).

## Testing Guidelines
- No automated test suite is present. Validate changes by running `jekyll serve` and manually spot-checking key pages and navigation.
- If you add new pages or data files, verify that links and menus render correctly in both `en/` and `kr/` sections.

## Commit & Pull Request Guidelines
- Recent commits use short, lowercase messages like `update registration` or `update rules`. Follow this pattern for consistency.
- Pull requests should include a brief description, list impacted pages (paths), and screenshots for visible UI changes.

## Content & Data Tips
- Keep data-driven content in `_data/*.yml` where possible and reference it in layouts for consistency across languages.
- Avoid editing `_site/`; always update source files and regenerate.
