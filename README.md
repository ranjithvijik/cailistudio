# CAILI AI Studio

CAILI AI Studio is a static landing page for the University of Baltimore's **Center for AI Learning and Community-Engaged Innovation (CAILI)**. It serves as a mission-led front door for responsible AI adoption across UBalt's Merrick School of Business, School of Law, College of Public Affairs, and Yale Gordon College of Arts & Sciences.

Built with Tailwind CSS (CDN) for rapid styling, a full UBalt brand system, and zero build dependencies.

## Project Structure

```text
CAILI AI Studio/
├── index.html                      # Main landing page (Tailwind CDN, inline styles)
├── README.md
├── design-spec.md                  # Original design specification
├── design-spec-v2.md               # Second iteration design spec
├── netlify.toml                    # Netlify static deploy config
├── styles.css                      # Legacy — not actively used (keep for reference)
├── .gitignore
├── instructions-generator/
│   └── index.html                  # Standalone tool page
├── ai-syllabi-policy-generator/
│   └── index.html                  # Standalone tool page
├── public/logo/
│   ├── logo-university-of-baltimore.png
│   ├── boodlebox-logo-dark.png
│   ├── boodlebox-logo-white.png
│   ├── boodlebox-all-dark.png
│   ├── boodlebox-all-white.png
│   └── boodlebox-avatar.png
├── Understanding Baltimores AI Ecosystem Report 2026- CAILI.pdf  # Persona research source
└── design/
    ├── .landing-page-superagent.png.icloud
    └── .use-case-superagent.png.icloud
```

## What This Project Includes

- **index.html** (1,305 lines, 120KB) — Complete landing page with:
  - Tailwind CSS via CDN with custom UBalt brand config
  - UBalt navy (#011221) + teal (#40C1BB) brand system
  - 6 persona cards (Civic Champion, Student Superuser, Adaptive Achiever, Prudent Professor, Hometown Hero, Labor Guardian) with deep-researched CAILI Solutions
  - 16-entry timeline from March 2023 through June 2026
  - Tool ecosystem section (ECON Simulator, ECON 606 Study Bot, OPM Simulator, QuantLab, Instructions Generator, AI Syllabi Policy Generator)
  - BoodleBox Integration with Coach Mode, FERPA/SOC2, 96% token reduction
  - UBalt official-style header (66px, 46px search icon, MENU at 24px/900 weight)
  - UBalt official footer with 5 social icons (Facebook, Instagram, YouTube, LinkedIn, TikTok)
  - 4-lens Responsible AI framework (Fairness, Transparency, Integrity, Community)
  - 8 AI classroom strategy cards with AI Assessment Scale (AIAS) integration
  - Timeline line gradient + 16 entries
  - Mega menu drawer with full UBalt navigation + colored CTAs
- **styles.css** — Legacy external stylesheet (not actively used; all styles are inline via Tailwind config + `<style>` block)

## UBalt Brand System

| Token | Value | Usage |
|---|---|---|
| `ubalt.navy` | `#011221` | Header, hero, footer, CTA sections |
| `ubalt.teal` | `#40C1BB` | Accent buttons, links, section labels, timeline |
| `ubalt.footer` | `#e8f8f7` | Footer copyright bar background |
| `text-display-xl` | `7rem / 900` | Hero heading |
| `text-display-lg` | `5rem / 900` | Section h2s (desktop) |
| `text-display-md` | `3.5rem / 900` | Section h2s (mobile) |

## Design Approach

- **Tailwind first**: The page uses Tailwind CDN with a custom `tailwind.config` extending colors, font sizes, and box shadows. A small inline `<style>` block adds custom CSS for `.reveal` animations, `.gradient-text`, `.browser-mockup`, and the `.timeline-line` pseudo-element.
- **UBalt identity**: The design faithfully reproduces the official ubalt.edu brand — navy background, teal accent, massive bold typography (80-119px), uppercase section headers, 1800px container with 80px gutters.
- **Research-backed**: All content is sourced from UBalt news articles, the CAILI persona report with Mindgrub, BoodleBox platform documentation, and EDUCAUSE AI ethical guidelines.

## Local Preview

```bash
python3 -m http.server 8000
# Open http://localhost:8000
```

## Deploying

This project deploys as a static site on **AWS Amplify**, connected to the `main` branch of the GitHub repository.

- **Live URL**: [https://main.dgiolfv4qrptj.amplifyapp.com](https://main.dgiolfv4qrptj.amplifyapp.com)
- **Build settings**: Amplify auto-detects the static site — no build command required, publish directory is `.`
- **Netlify**: The included `netlify.toml` also supports Netlify deployment as an alternative.

The `netlify.toml` file is pre-configured for root-level deploy if using Netlify.

## Credits

Programmed for CAILI by Jenish Amatya and Ranjith Keerikkattil. Built with research from the "Understanding Baltimore's AI Ecosystem" report with Mindgrub, official UBalt news sources, and BoodleBox platform documentation.
