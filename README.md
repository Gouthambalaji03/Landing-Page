## Trabook Landing Page (HTML/CSS)

This project is a responsive single–page landing built with semantic HTML and modern CSS (no frameworks). It reproduces the provided UI, including the hero section, feature/deals blocks, testimonials, blog, and a subscribe banner.

### Preview

Open `index.html` directly in any modern browser, or use a lightweight static server (e.g., VS Code Live Server) for a smoother experience.

### Tech stack

- HTML5 (semantic structure)
- CSS3 (flexbox/grid, custom properties, media queries)
- Google Fonts: Poppins, Volkhov

### Project structure

```
Landing Page/
├─ index.html          # Page markup
├─ app.css             # Global styles & responsive rules
├─ assets/
│  ├─ images/          # Illustrations & decorative SVG/PNGs
│  └─ icons/           # Small UI icons (svg)
└─ README.md
```

### Getting started

1. Clone or download this folder.
2. Double‑click `index.html` (or right‑click → "Open with Live Server").
3. All images and icons are referenced relatively from `assets/`.

#### Clone via Git

```bash
# with HTTPS
git clone https://github.com/<your-username>/<your-repo>.git

# or with SSH
git clone git@github.com:<your-username>/<your-repo>.git

cd <your-repo>
# open in VS Code (optional)
code .
```

### Deploy to Netlify

You can deploy this static site in a few clicks:

1. Push your project to GitHub/GitLab/Bitbucket
2. Sign in to [Netlify](https://www.netlify.com/)
3. New site → Import from Git
4. Select your repository
5. Build settings:
   - Build command: (leave empty — this is a static site)
   - Publish directory: `.` or the folder that contains `index.html`
6. Deploy

Alternative (drag & drop):

1. Run `zip` on the project folder (including `index.html`, `app.css`, `assets/`)
2. Go to Netlify → Sites → "Deploy site by dragging and dropping your site folder"
3. Drop the ZIP or the folder to upload

Netlify will assign a URL like `https://your-site-name.netlify.app`. You can rename the site from Site settings → Site details.

### Key features

- Responsive hero with circular accent and centered figure
- Navigation with anchor links to each section
- Cards/Grids built with CSS Grid (auto switches to 1–2 columns)
- Subscribe banner with layered background doodles
- Footer alignment with left copyright and right “Terms & Conditions”

### Responsiveness

The layout is tuned for common breakpoints:

- `≤ 1024px` (tablet landscape): hero stacks, grids adapt to 2 cols
- `≤ 768px`  (tablet portrait): centered CTAs, single‑column content
- `≤ 640px`  (mobile): compact typography, single‑column sections,
  hidden floating badges, full‑width forms

You can adjust these in `app.css` (search for `@media` blocks and the
`.hero-grid`, `.feature-grid`, `.card-grid`, `.testimonials-grid`, and
`.subscribe-*` rules).

### Customization

- Primary color(s) are defined as CSS variables at the top of `app.css`:
  ```css
  :root {
    --brand: #ff7a1a;
    --brand-600: #ff6a00;
    --text: #0f1828;
    --text-dim: #6b7280;
    --bg: #ffffff;
  }
  ```
- Update fonts in the `<head>` of `index.html` if you prefer a different typeface.
- Swap or add images in `assets/images` and update the corresponding `src` attributes.

### Known tips

- If you need a mobile menu, add a hamburger toggle and show/hide `.primary-nav` below `640px`.
- If scroll‑to anchors overlap with the sticky header, add `scroll-margin-top` to section roots.

### Credits

- UI inspired by the provided design reference.
- Icons and illustrations in `assets/` are for demo purposes.

### License

This project is provided for educational/demo use. Adapt freely for your own projects.


