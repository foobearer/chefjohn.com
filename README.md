# Chef John C. Paragas — Portfolio

A single-page culinary portfolio: video hero, floating plate cutouts,
scroll-driven editorial sections.

**Live site:** https://www.chefjohn.fyi

## Structure

| Path                 | What it is                                        |
|----------------------|---------------------------------------------------|
| `index.html`         | The entire site — markup, styles and script       |
| `cutouts/`           | 12 circular plate cutouts (transparent WebP)      |
| `plates/`            | 12 rectangular editorial photos (WebP)            |
| `video/`             | Hero footage `kitchen.mp4` + `poster.jpg`         |
| `favicon.*`          | Chef's toque tab icon                             |

## Editing

- **Copy** — all text lives directly in `index.html`.
- **Photos** — replace a file in `plates/` keeping the same filename.
- **Floating plates** — edit the `FIELD` table near the top of the `<script>`
  block. Each entry is `{id, x, y, w, d}`: filename, position in %, width in
  vmin, and depth from 0 (far, soft, slow) to 1 (near, sharp, fast).
- **Hero video** — swap `video/kitchen.mp4`, keeping it small (<1 MB) and muted.

Built with GSAP + ScrollTrigger and Lenis, loaded from CDN. No build step.
