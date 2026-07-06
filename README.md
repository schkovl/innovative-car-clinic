# Innovative Car Clinic — Website

Static site migrated from Wix (`innovativecarclinic.wixsite.com/innovative-car-clini`).
Plain HTML/CSS/JS — no build step, no dependencies.

## Pages

| File | Page |
|------|------|
| `index.html` | Home (hero, intro, services overview, CTA) |
| `services.html` | Services (5 service details) |
| `about.html` | About Us |
| `faq.html` | FAQ (8 questions, accordion) |
| `contact.html` | Contact (details + form) |

## Deploy to Replit

1. Create a new Repl → choose the **HTML/CSS/JS** (static) template.
2. Upload all files and the `assets/` folder (drag-and-drop into the Files pane).
3. Hit **Run** — Replit serves `index.html` automatically.
4. To publish: **Deploy → Static Deployment** (free tier works for static sites).

## Local preview

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Notes

- **Contact form** opens the visitor's mail client (`mailto:` to info@innovativecarclinic.ca) because static hosting has no backend. To get submissions without email clients, swap in a form service (e.g. Formspree): change the `<form>` tag to `action="https://formspree.io/f/YOUR_ID" method="POST"` and remove the submit handler in `script.js`.
- Images in `assets/` were carried over from the original Wix media library (Adobe Stock assets licensed by the business).
- Fonts: Archivo (display) + Inter (body) from Google Fonts — substitutes for the Wix-licensed Avenir/Lulo Clean.
- Original Wix gold accent `#938533` kept as the brand accent.
- The original site is currently `noindex` (unpublished Wix free tier); once the new site is live on a real domain, add a sitemap and remove nothing — no `noindex` is set here.
