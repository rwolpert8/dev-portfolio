# Ryan Wolpert — Developer Portfolio

A responsive personal portfolio in plain HTML, CSS, and JavaScript. Features PetSnap, Coverage Copilot, and HighHeat, plus background, résumé, and contact links.

## Preview

Run `python -m http.server 8000` from this directory and visit http://localhost:8000. You can also open `index.html` directly. No build step or dependencies are required.

## Design and behavior

- Near-black background, orange accents, and Space Grotesk / Manrope typography.
- The hero slogan uses a fixed Space Grotesk font.
- Responsive layouts, semantic sections, visible keyboard focus, and a skip link.
- Fonts load from Google Fonts with local fallbacks. The rest of the page requires no external assets.

## Editing

- `index.html`: copy, projects, links, and metadata.
- `styles.css`: palette, typography, layout, and responsive rules.
- `script.js`: footer year.
- `resume.md`: source résumé. The About section links to the hosted Google Drive résumé.

PetSnap’s featured section links to its public Railway demo alongside the GitHub repository. The project graphic is a pipeline illustration, not a screenshot of the app.

## Hosting

Deploy the directory to any static host, including GitHub Pages. No compilation or server-side configuration is needed.
