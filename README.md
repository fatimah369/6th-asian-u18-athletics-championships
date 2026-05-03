# The 6th Asian U18 Athletics Championships — Project Showcase

Single-page showcase site, built and delivered by **Mode Event**, documenting the operational scope and delivery of *The 6th Asian U18 Athletics Championships* (Saudi Arabia, 2025).

The page is served as a single static `index.html` file:

- Hero with the official championship logo (embedded as a base64 PNG)
- Project overview
- Animated stats bar (29 countries, 700+ athletes, 7 days, 70 performers, 1 championship)
- Six-card "Our Role" deliverable grid
- Five-stage execution timeline
- Impact pull-quote
- Mode Event footer with a "Work With Us" CTA

## Design system

- **Typography** — Google Fonts: Barlow Condensed (heavy) for headings, Barlow (light–medium) for body
- **Colors** — extracted strictly from the brand `.pptx` file (theme accents + explicit slide colors)
- **Logo** — extracted from the brand `.pdf` file and embedded directly inside `index.html` as a base64 PNG
- **No frameworks** — vanilla HTML + CSS + a small inline `<script>` for reveal-on-scroll and the animated counters
- **No emojis** — icons are inline SVGs
- **Responsive** — mobile, tablet, desktop breakpoints
- **Accessibility** — respects `prefers-reduced-motion`, semantic landmarks (header / section / footer), descriptive alt text

## Running locally

The site is one static file. Either open `index.html` directly in a browser, or serve it:

```bash
python -m http.server 5050
# then visit http://localhost:5050
```

## Deployment

Works on GitHub Pages with no build step. Enable Pages on the `main` branch (root) and the site is live at the project's Pages URL.
