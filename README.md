# zackreyrussell.com

Source code for my personal portfolio site, built to showcase my work as a Senior Data Analyst and Analytics Engineer.

## What's here

A custom-built, single-page portfolio site covering experience, project case studies, and contact information. No framework, no template, built from scratch with hand-rolled CSS and a small amount of vanilla JS for scroll animations and form handling.

- **Hero and navigation** — fixed nav with smooth scroll, animated noise overlay, and a layered radial-gradient background
- **Projects section** — five project cards covering ETL pipelines, product adoption metrics, Mixpanel implementation, multi-source data integration, and subscription funnel analytics
- **Case studies** — two deep-dive pages on personal research projects:
  - **Awards Predictability Analysis** ([`awards.html`](awards.html)) — which major film award show best predicts the Oscar for Best Picture, built on a custom relational database spanning 7 award shows and 2,400+ nomination records ([database repo here](https://github.com/ZackRussell/filmAwardAnalysis))
  - A second case study ([`case2.html`](case2.html))
- **Experience timeline** — Instinct Science and VetMedux, with specific, validated outcomes rather than generic role summaries
- **Contact form** — wired to Netlify's built-in form handling, no backend or exposed API keys required

## Stack

Plain HTML/CSS/JS. Google Fonts (DM Serif Display, DM Mono, DM Sans). `IntersectionObserver` for scroll-triggered fade-ins. Netlify Forms for the contact form submission, with a honeypot field for basic spam protection.

## Structure

```
index.html          # Main landing page
awards.html          # Case study: Awards Predictability Analysis (overview)
awards-bafta.html    # Per-show deep dive: BAFTA
awards-cc.html       # Per-show deep dive: Critics Choice
awards-dga.html      # Per-show deep dive: DGA
awards-gg.html       # Per-show deep dive: Golden Globes
awards-pga.html      # Per-show deep dive: PGA
awards-sag.html      # Per-show deep dive: SAG
case2.html           # Second case study
```

## Running it locally

No build step. Open `index.html` in a browser, or serve the folder with any static file server:

```bash
python3 -m http.server 8000
```

## Deployment

Hosted on Netlify, deployed from this repo.
