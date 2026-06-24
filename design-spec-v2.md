# CAILI AI Studio — Design Evolution (v2 → Current)

This file documents the evolution of the CAILI AI Studio landing page from the v2 design specification to the current production version.

## Timeline of Design Changes

### Phase 1: Original Build (2025)
- Superagent.com-inspired design: purple-to-pink gradients, beige/cream base (#F9F5EB), light pastel cards
- Two-column feature panels: MBA AI Workflows + BoodleBox Integration
- Basic use-case grid with MBA and Law cards
- Simple ethics section with a single pass/fail list
- Scroll-triggered reveal animations

### Phase 2: UBalt Brand Overlay
- Shifted from superagent aesthetic to ubalt.edu brand
- Replaced purple-pink with navy (#011221) + teal (#40C1BB) color system
- Replaced beige with white + slate-50 backgrounds
- Added UBalt official header (navy, 66px, logo + search + MENU)
- Added UBalt official footer with social icons
- Implemented mega menu drawer with full UBalt navigation (Academics, Admission & Aid, Student Life, About, Schools, colored CTAs)
- Replaced gradient accent from purple-pink to teal-cyan (#40C1BB → #5EEAD4 → #2DD4BF)

### Phase 3: Container Width Overhaul
- Changed from `max-w-7xl` (1280px) to `max-w-[1800px]` to match ubalt.edu
- Changed horizontal padding from 32px to 80px (desktop), matching UBalt's `.container` 80px gutter
- Tightened section spacing from `py-24` (96px) to `py-20` (80px)
- Reduced card shadows from heavy `0 4px 20px` to subtle `0 1px 3px`

### Phase 4: Research-Driven Content Expansion

**Persona Compass Section (new):**
- Added 6 persona cards based on "Understanding Baltimore's AI Ecosystem" report with Mindgrub
- Persona color coding: Active (sky), Hesitant (amber), Resister (pink)
- Each card: initials avatar, quote, background, needs & fears, CAILI Solution description
- Common Themes chips (AI as Calculator, AI Training Lacking, Environmental Impact)
- What Now callout with Dr. Stansbury's contact
- Where We Are / Where We Want to Be cards

**Timeline Section (new):**
- 16 entries from March 2023 through June 2026
- Sources: UBalt official timeline PDF, CAILI Year One article, BoodleBox partnership article, AI Summit announcements, Technical.ly coverage

**BoodleBox Section Enhanced:**
- Added real BoodleBox features: Coach Mode, Custom AI Assistants, Knowledge Foundation
- FERPA compliant + SOC 2 certified
- 96% token reduction technology
- Lifelong portability (students keep access after graduation)
- "Data stays yours — never trains models on user content"
- Mockup now shows: 4 shared rooms (including AI Navigator Cohort), 4 active model tags (GPT-4o, Claude, Gemini, Perplexity), 3-message chat

**What We Offer Cards:**
- Added AI-Enabled Business Accelerator (9-week program, 8 founders, healthcare/energy/education/housing)
- Added AI Navigator Fellows to Faculty Education card

**Use Cases Expanded:**
- Added AI-Enabled Venture Building card (AI Accelerator category)
- Added real tool links: ECON Simulator (Amplify), ECON 606 Study Bot (BoodleBox), OPM Simulator (Streamlit), QuantLab (Streamlit)

### Phase 5: Persona CAILI Solutions Deep Research
Each persona's CAILI Solution block was rewritten with specific, referenced program details:

| Persona | Enhancement |
|---|---|
| Civic Champion | Community-Grounded Compass with Mindgrub, "over-eager assistant" philosophy, 4-lens framework |
| Student Superuser | ECON 606 Study Bot (multi-agent), EconSim (78 modules + FRED), Coach Mode, process files |
| Adaptive Achiever | Anti-hallucination design (course-grounded bots with citations), Coach Mode metacognitive skills |
| Prudent Professor | AIAS-based Policy Generator, Instructions Generator, AI Navigator Fellows program |
| Hometown Hero | Live Prototypes + AI Business Accelerator, Community Lens, free BoodleBox |
| Labor Guardian | "Enhance—rather than replace" philosophy, transparency architecture, AI Accelerator creates jobs |

### Phase 6: Typography Overhaul
- Updated h2s from `text-3xl md:text-4xl font-bold` to `text-display-md md:text-display-lg font-black uppercase tracking-tight`
- Added `display-xl` (7rem), `display-lg` (5rem), `display-md` (3.5rem) to Tailwind config
- Hero h1: `text-display-xl` with 2-line split pattern ("CAILI AI" + "Studio")
- All section h2s now uppercase matching ubalt.edu

### Phase 7: Responsible AI Section Deep Research

**Intro paragraph:** Now references UBalt Generative AI Guidelines (Office of Academic Affairs), EDUCAUSE AI Ethical Guidelines, and 6 personas

**4-lens cards enhanced:**
- Fairness: "Check for missing voices, uneven impact — use AI to widen perspective, not narrow it"
- Transparency: "Every CAILI Study Bot cites exactly which teaching materials inform its responses — no black boxes"
- Integrity: "BoodleBox process-file submission and Coach Mode make AI use visible and auditable"
- Community: "The Community Lens ensures tools are built with communities, not just for them"

**Do/Don't guidance:** Expanded from 3+3 to 4+4 items, each tied to specific persona voices (Civic Champion's "over-eager assistant", Prudent Professor's insistence on clear guidelines, Labor Guardian's concern about exploitation, Adaptive Achiever's boundary of completing personal notes first)

**Classroom strategies:** Expanded from 4 cards to 8 cards with unique accent colors:
- Clarify Expectations (emerald), AI Assessment Scale (blue), Design for Process (amber), Personalize & Localize (purple), Intentionally Integrate AI (rose), Rethink Mastery (cyan), Emphasize Iteration (orange), Support Multiple Modalities (indigo)

**Policy links:** Added UBalt Generative AI Guidelines PDF link (developed with Academic Affairs)

### Phase 8: Navigation Redesign
- Header height: `h-16` → `height:66px` (matches ubalt.edu)
- Search icon: 24px → 46px (matches ubalt.edu)
- MENU button: `text-xs font-bold` → `font-black text-2xl uppercase` (24px/900 weight, matches ubalt.edu)
- Padding: `px-7 py-4` on MENU button (matches UBalt's generous padding)

### Phase 9: Contrast Optimization
- All `text-slate-500` → `text-slate-600` (~70 instances) for WCAG-AA compliance
- Hero body: `text-white/50` → `text-white/65`
- Hero subtitle: `text-white/80` → `text-white/90`
- Bold highlights in hero: `text-white/80` → `text-white`
- Gradient: 2-stop → 3-stop for more vivid rendering added `background-clip: text` standard property

## Current File Metrics

- **File size**: 120KB
- **Lines**: 1,305
- **Sections**: 10 content sections + header + footer + scripts
- **Links**: 60+ hrefs (internal anchors + external ubalt.edu URLs + tool URLs)
- **Tags**: Balanced (10 section, 292 div, 4 details/summary, all verified)
- **Styling**: Tailwind CDN + 70-line inline `<style>` block (animations, gradient, timeline, mockup, scrollbar)

## Key Design Decisions

1. **Single file**: Everything in index.html — Tailwind CDN eliminates build step, inline `<style>` for custom CSS that Tailwind can't express (pseudo-elements, keyframes)
2. **No javascript framework**: Vanilla JS for nav drawer, reveal animations, text rotator, and use-case filters
3. **UBalt fidelity over innovation**: The design intentionally matches ubalt.edu closely — 1800px container, 80px gutters, 66px header, 46px search icon, 24px/900 weight MENU
4. **Content sourced from real UBalt research**: All CAILI program details, BoodleBox features, and persona descriptions are sourced from:
   - UBalt official news articles
   - BoodleBox platform docs
   - CAILI persona report with Mindgrub
   - EDUCAUSE AI ethical guidelines
   - AI Assessment Scale framework
   - UBalt Generative AI Guidelines
