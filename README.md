# WISMUN

A React website for the WISMUN website

## Pages

| Route | Description |
|-------|-------------|
| `/` | Home — hero, stats, about, committees overview, CTA |
| `/register` | Delegate registration form with validation |
| `/brochure` | Full programme: committees, schedule, rules, FAQs |
| `/contact` | Team contacts + inquiry form |

## Tech Stack

- **React 18** with React Router v6
- **CSS custom properties** (no Tailwind / CSS-in-JS)
- Google Fonts: Playfair Display, Inter, Space Mono
- No external UI libraries

## Getting Started

```bash
# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build
```

## Project Structure

```
src/
├── App.js                  # Router + layout shell
├── index.js                # React entry point
├── index.css               # Global styles & design tokens
├── components/
│   ├── Navbar.js / .css    # Fixed navigation bar
│   └── Footer.js / .css    # Site footer
└── pages/
    ├── Home.js / .css      # Landing page
    ├── Register.js / .css  # Registration form
    ├── Brochure.js / .css  # Conference brochure
    └── Contact.js / .css   # Contact page
```

## Customisation

- Update conference dates, venue, and pricing in the relevant page files.
- Replace placeholder emails (`secretariat@munvi.org`, etc.) with real addresses.
- Add the real committee topics once finalised.
- Connect the forms to a backend / email service (e.g. EmailJS, Formspree, or a custom API).

## Deployment

Works with any static host — Vercel, Netlify, GitHub Pages.

For GitHub Pages, add `"homepage": "https://<your-org>.github.io/<repo-name>"` to `package.json` and run:

```bash
npm install --save-dev gh-pages
npm run build
npx gh-pages -d build
```

---

