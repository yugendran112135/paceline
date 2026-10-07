# Paceline — Running retail website

Responsive two-page site (Home + About) built with semantic HTML, a single CSS file and vanilla JS. No build step.

## Run locally
```bash
git clone <your-repo-url> && cd paceline
python3 -m http.server 8000     # or: npx serve .
# open http://localhost:8000
```
Opening `index.html` directly in a browser also works.

## Features
- Sticky header, mobile hamburger menu (Esc to close)
- Hero slider: auto-advance, pauses on hover/focus, dot controls
- New-arrivals filter tabs, wishlist toggles, animated stat counters
- Newsletter form with validation + live-region feedback

## Performance & a11y
- Images converted to WebP, explicit width/height (no layout shift), lazy-loaded below the fold
- Skip link, landmarks, visible focus, ARIA tabs/pressed states, `prefers-reduced-motion` support
- Mobile-first CSS grid/flex; breakpoints at 640 / 900px

## Deploy
Static site — drag the folder into Netlify, or `vercel --prod`, or enable GitHub Pages.

## Structure
```
index.html  about.html
css/styles.css   js/main.js   assets/img/*.webp
```
