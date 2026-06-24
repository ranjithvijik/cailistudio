# CAILI AI Studio

CAILI AI Studio is a static landing-page prototype for the University of Baltimore's Center for AI Learning and Community-Engaged Innovation. The site is designed as a mission-led front door for responsible AI adoption across the Merrick School of Business, the School of Law, and the College of Public Affairs.

This version is built as a plain static site so it can be deployed quickly for demos without introducing framework overhead or visual drift.

## What This Project Includes

- A full landing page in `index.html`
- All styling and motion in `styles.css`
- University of Baltimore and BoodleBox logo assets in `public/logo/`
- Design reference screenshots in `design/`
- Netlify configuration in `netlify.toml`

## Why It Is Structured This Way

This project is intentionally simple:

- No build step
- No framework dependency
- No bundler requirement
- Easy GitHub upload
- Easy Netlify deployment

That makes it the safest setup for preserving the exact current content, layout, animation, and styling during deployment.

## Project Structure

```text
CAILI-ai-studio/
├── index.html
├── styles.css
├── netlify.toml
├── README.md
├── public/
│   └── logo/
├── design/
├── design-spec.md
└── design-spec-v2.md
```

## Local Preview

Because this is a static site, you can preview it with any lightweight local server from the project root.

Example:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deploying To GitHub

If the project has not been committed yet:

```bash
git add .
git commit -m "Initial CAILI AI Studio landing page"
```

Then connect the local repository to GitHub:

```bash
git remote add origin <your-github-repo-url>
git push -u origin main
```

## Deploying To Netlify

This repository is already configured for a root-level static deploy.

Netlify settings:

- Build command: leave blank
- Publish directory: `.`

If you import the GitHub repository into Netlify, it should detect `netlify.toml` automatically and publish the site from the root folder with no additional build setup.

## Deployment Checklist

Before sharing the demo:

- Confirm `index.html` loads correctly from the root
- Confirm logos load from `public/logo/`
- Confirm the ethics interactions behave as expected in a modern browser
- Confirm anchor links and external links open correctly
- Confirm the site looks right on both desktop and mobile

## Browser Notes

The site uses modern CSS for some of the ethics interactions, including `:has(...)`, masks, gradients, and layered motion effects. Current versions of Chrome and Safari handle these well. Older browsers may still render the page, but some advanced interactions may appear more basic.

## Notes For Demo Use

- This is a prototype, not a production application
- The login button currently routes to the public BoodleBox site
- The deployment is optimized for visual fidelity and ease of presentation

## Credits

Concept and prototype implementation for CAILI AI Studio by Jenish Amatya.
