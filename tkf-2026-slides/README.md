# TechKnowFile 2026 Slides

[Quarto](https://quarto.org/) [Reveal.js](https://quarto.org/docs/presentations/revealjs/) slide deck for "Automated observability with Puppet in a zero-trust environment".

## Prerequisites

- Quarto CLI installed (`quarto --version`)
- A web browser for preview

## Project layout

- Source deck: `index.qmd`
- Theme: `dracula` and `custom.scss`
- Project config: `_quarto.yml`
- Rendered output directory: `output_html/`

## Render HTML

From this directory (`tkf-2026-slides`):

```bash
quarto render index.qmd --to revealjs
```

Generated file:

- `output_html/index.html`

## Live preview (auto-reload)

```bash
quarto preview index.qmd
```

Quarto starts a local preview server and rebuilds when files change.

## Render all project files

If you later add more `.qmd` files and want to build everything:

```bash
quarto render
```

## Optional: PDF export workflow for Reveal.js

1. Render the deck.
2. Open `output_html/index.html` in a browser with `?print-pdf`.
3. Use browser print to save PDF.

Example URL pattern:

```text
file:///.../tkf-2026-slides/output_html/index.html?print-pdf
```

