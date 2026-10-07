# Manish Modwani: portfolio

**Live:** https://manimod7.github.io/ · **GitHub:** https://github.com/manimod7 · **LinkedIn:** https://www.linkedin.com/in/manish-modwani

Personal portfolio of Manish Modwani, Software Development Engineer II at Amazon (Bangalore), previously at PayPal. It is a single static page with no framework, no build step and no dependencies other than Google Fonts.

---

## Contents

1. [What is on the site](#what-is-on-the-site) · 2. [Projects](#projects) · 3. [Design](#design) · 4. [Files](#files) · 5. [Edit and deploy](#edit-and-deploy) · 6. [Tech notes](#tech-notes) · 7. [FAQ](#faq)

## What is on the site

| Section | Content |
| --- | --- |
| Overview | Intro, role and location, live clock, headline stats |
| Featured | Highlighted work, with a small interactive reconciliation demo |
| Experience | Amazon and PayPal roles, in tabs |
| Impact | What I delivered at Amazon and at PayPal |
| Projects | Chase and SwingLab, with a details panel and live demo links |
| Stack | Languages, data engineering, cloud and tools |
| Recognition | Awards, including Top Performer at Amazon (2026) |
| Contact | Email, LinkedIn, GitHub, resume |

The **reconciliation demo** shows how a variance between Amazon's books and a partner's report is found and closed with an adjustment booking. It uses deliberately simple round numbers so the arithmetic is easy to check: books 1,000 units / 10,000.00 gross / 1,000.00 commission against a partner report of 990 / 9,900.00 / 990.00, so the variances are -10 units, -100.00 gross and -10.00 commission, and net to book is 9,000.00 against 8,910.00, a variance of 90.00 EUR. The figures are illustrative, not real data.

## Projects

Click a project card to open a panel with what it does, how it works, key numbers and links.

- **Chase**: ball-by-ball win probability for T20 cricket. Live: https://manimod7.github.io/chase/ · Source: https://github.com/manimod7/chase
- **SwingLab**: a swing lab for a 3D-printed VR cricket bat on Meta Quest 3. Live: https://manimod7.github.io/swinglab/ · Source: https://github.com/manimod7/swinglab

Each project has its own detailed README.

## Design

- Minimal bento-grid layout for a software-developer portfolio: monospaced labels, tight type, one accent colour.
- Fonts: Archivo (headings), Figtree (body), JetBrains Mono (labels).
- **Dark theme:** near-black with orange accent. **Light theme:** "Warm Paper", a warm cream with burnt-orange accent.
- Follows the system theme by default; the sun/moon button switches manually and the choice is remembered in the browser. The two project apps use the same toggle.
- Responsive down to phone width; respects reduced-motion settings.

## Files

```
index.html                  the whole site (HTML, CSS and JavaScript in one file)
Manish_Modwani_Resume.pdf   linked from the page
README.md                   this file
```

## Edit and deploy

The site is served by GitHub Pages from the `main` branch root of the repository `manimod7/manimod7.github.io`.

1. Open the repo on GitHub and click `index.html`, then the pencil icon.
2. Edit and click **Commit changes**.
3. Wait a minute or two, then hard refresh (Ctrl+Shift+R) https://manimod7.github.io/.

To replace the resume, use **Add file, Upload files** with the same name `Manish_Modwani_Resume.pdf`.

## Tech notes

- Theming uses CSS custom properties on `:root`, overridden under `prefers-color-scheme: dark` and `[data-theme]`.
- Project panels use the native `<dialog>` element (`showModal()`), which gives focus trapping and Esc to close for free.
- No cookies, analytics or trackers. The only stored value is the theme choice in `localStorage`.

## FAQ

**Why one file?** It is easy to host, edit and review, and loads fast.

**Why are the demo numbers so simple?** So anyone can verify the calculation at a glance.

**Can I reuse the design?** Please ask first, and do not reuse the personal content.

**How do I report a problem?** Open an issue on https://github.com/manimod7/manimod7.github.io or email me via the Contact section.
