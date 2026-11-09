# Shameera Rathnayaka — Personal Website (`shameera.dev`)

A zero-dependency, SEO-optimized personal website themed with the official **Catppuccin** color palette (`Mocha` default, `Macchiato`, `Frappé`, and `Latte`).

## Project Structure

- `index.html` — Semantic HTML5 content, Open Graph tags, and Schema.org `Person` JSON-LD structured data.
- `styles.css` — Catppuccin design tokens (`@layer theme`), base resets (`@layer base`), and component styles (`@layer components`).
- `robots.txt` & `sitemap.xml` — Search engine crawler configuration (update `https://shameera.dev/` to your custom domain once deployed).

## Local Preview

Run any static file server from this directory:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## How to Maintain & Update Content

1. **Add or Edit a Career Role**: Open `index.html` under `<!-- 01 // Career Trajectory -->` and duplicate a `<div class="timeline-item">...</div>` block.
2. **Add an Open Source Project**: Open `index.html` under `<!-- 02 // Open Source & Personal Projects -->` and add an `<article class="craft-card">...</article>` block.
3. **Change Default Catppuccin Flavor**: In `index.html`, change `<html lang="en" data-flavor="mocha">` and the fallback in the `<head>` script from `"mocha"` to `"macchiato"`, `"frappe"`, or `"latte"`.

## Deployment

Because there is no build step, you can deploy the repository root directly to:
- **GitHub Pages** (Settings → Pages → Deploy from branch `main` / `/ (root)`)
- **Cloudflare Pages** (Framework preset: `None`, Build output directory: `/`)
- **Firebase Hosting** or **Google Cloud Storage**
