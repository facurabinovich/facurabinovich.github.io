# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Facundo Rabinovich's personal portfolio site, hosted on GitHub Pages (`facurabinovich.github.io`) and built with Jekyll using the `jekyll-theme-minimal` theme (via `_config.yml`). There is no build tooling, package manager, or test suite — GitHub Pages compiles the Jekyll site automatically on every push to the deployed branch. To preview locally you'd need a standard `jekyll serve` / Bundler setup, but no Gemfile currently exists in the repo, so there is no local build command configured.

## Architecture

- `_config.yml` — site title, description, logo path, and theme selection (`jekyll-theme-minimal`). Keep `description` free of raw HTML (e.g. no `<br>`) — it renders inside the sidebar `<p>` and stray markup breaks the layout.
- `_layouts/default.html` — the page shell: sidebar (`<header>`) with title, profile photo, description, and hardcoded LinkedIn/GitHub SVG social links, plus the `<section>{{ content }}</section>` for page markdown. Loads Google Fonts (Inter) and devicons (via jsdelivr CDN) in `<head>`. Contains an inline `<style>` block after all stylesheet `<link>` tags — this is the **guaranteed override layer** (see CSS gotcha below), not just decoration. There is intentionally no `<footer>` — it was removed because it overlapped the sidebar content.
- `assets/css/style.scss` — imports the theme (`@import "{{ site.theme }}"`) then layers dark-mode and component styles on top: sidebar, social links, project nav pills, project cards, tech badges, project buttons, image galleries.
- `index.md` — the homepage content, with `layout: default` in front matter. Structured as a `.project-nav` pill bar linking to `.project-card` divs (each with `markdown="1"` so embedded Markdown still renders inside HTML divs), tech-stack badges using devicon `<i>` classes, and an "About Me" section.
- `sample_page.md` — unused template boilerplate left over from the original theme fork; not linked from the nav.
- `images/`, `gifs/`, `pdf/` — static assets referenced from `index.md` (project screenshots/demos).

## Critical CSS gotcha (GitHub Pages SCSS compiler)

CSS custom properties (`var(--x)`) combined with `!important` do **not** reliably override the theme's compiled CSS on GitHub Pages' Jekyll/SCSS pipeline. When touching styles:

1. Use hardcoded hex values in `style.scss` (e.g. `#0d1117`), never `var(--bg-primary)`.
2. Duplicate any style rule that must win against the theme as an inline `<style>` block in `_layouts/default.html`, placed after all `<link>` tags — that inline block is the actual override guarantee, `style.scss` alone is not sufficient for contested rules (bold text color, nav pills, card backgrounds, etc.).

This means style changes to shared/critical rules typically require editing **both** `assets/css/style.scss` and the inline `<style>` block in `_layouts/default.html` to stay in sync — check both when making dark-mode or layout changes.

## Adding a new project card

Follow the existing pattern in `index.md`:
1. Add a pill link to `.project-nav` at the top (`<a href="#slug">emoji Name</a>`).
2. Add a `<div class="project-card" id="slug" markdown="1">` block with an `<h1>` title, feature list, `.tech-stack` badges (use `devicon-*` classes where available, plain text span otherwise), `.project-actions` buttons (Live Demo / GitHub Repo), and optional `.project-gallery` images/GIFs.
3. Image paths for local assets use `images/name.png?raw=true`; external repo GIFs are pulled from `raw.githubusercontent.com`.
