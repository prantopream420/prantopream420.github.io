# Pranto Pream — Portfolio Site

A modern, dark-themed personal portfolio website for Pranto Pream, featuring IT expertise, photography, and open-source projects.

## Structure

```
portfolio-site/
├── index.html          # Main page (single-page application)
├── styles.css          # All styles with CSS variables, animations, responsive design
├── script.js           # Interactivity: navbar, gallery filter, form, scroll animations
├── images/
│   ├── profile.jpg     # Profile photo
│   ├── logo.png        # Logo/brand graphic
│   └── gallery/        # Event photography gallery (8 images)
│       ├── gallery-1.jpg through gallery-8.jpg
└── projects/           # (available for future project detail pages)
```

## Sections

- **Hero** — Name, tagline, stats, profile photo with floating social badges, CTA buttons
- **About** — 4 cards: Tech, Photography, Open Source, Community
- **Skills** — 6 categories: IT Support, Linux/Open Source, Android/AOSP, Programming, Creative/QA
- **Projects** — 6 GitHub projects with tech tags and links
- **Gallery** — Filterable event photography (club, concert, project show)
- **Contact** — Info cards + functional form + social links

## Running Locally

Open `index.html` in any browser, or serve locally:
```bash
# Any static server
python3 -m http.server 8080 --directory portfolio-site
# or
npx serve portfolio-site
```

## Design Features

- Dark theme with purple/teal gradient accents
- Floating gradient orbs with parallax scroll
- Scroll-triggered fade-in animations
- Responsive mobile-first layout
- Glassmorphism navbar with backdrop blur
- Gallery with category filtering
- Contact form with success state
- All links point to real GitHub/social profiles
