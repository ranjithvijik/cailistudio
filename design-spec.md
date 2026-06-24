# CAILI AI Studio — Design Specification

## Brand System

- **Primary dark**: Navy `#011221` — header, hero, footer, CTA sections, button backgrounds
- **Primary accent**: Teal `#40C1BB` — CTAs, links, section labels, timeline dots, hover states
- **Footer accent**: Light teal `#e8f8f7` — footer copyright bar (matches ubalt.edu `main-footer__copyright`)
- **Background**: White `#ffffff` for content sections; `#f5f7fa` (slate-50) for alt sections
- **Selection**: Teal tint `bg-[#40C1BB]/20 selection:text-[#011221]`

## Typography

- **Font stack**: `Inter, system-ui, -apple-system, sans-serif` (Google Fonts)
- **Display XL**: `7rem / 0.95 leading / -0.03em tracking / 900 weight` — hero heading
- **Display LG**: `5rem / 1 leading / -0.02em tracking / 900 weight` — section h2s (desktop)
- **Display MD**: `3.5rem / 1.05 leading / -0.02em tracking / 900 weight` — section h2s (mobile)
- **Section h2s**: UPPERCASE, font-black, uppercase tracking-tight (matching ubalt.edu)
- **Body**: Inter regular/semibold, sizes from text-xs to text-lg, slate-600 for contrast
- **Gradient text**: `linear-gradient(135deg, #40C1BB 0%, #5EEAD4 50%, #2DD4BF 100%)` with `background-clip: text`

## Layout

- **Container**: `max-width: 1800px`, `padding: 0 80px` (desktop), responsive down to 20px on mobile
- **Section spacing**: `py-20` (80px) uniform top/bottom padding, matching ubalt.edu
- **Card shadows**: Minimal `0 1px 3px rgba(0,0,0,0.04)` — clean institutional style
- **Header**: Fixed, 66px height, navy background, logo left + 46px search icon + MENU (24px/900 weight)

## Sections (in page order)

1. **Hero**: Navy bg, 144px padding, teal label, 2-line split h1 ("CAILI AI" / "Studio" with gradient), subtitle, body text, two CTAs (teal primary + outline secondary), 4 highlight cards (white, 2xl rounded, hover lift)
2. **Ecosystem**: Tool grid with MBA tools (4 cards) + Faculty tools (2 split cards), each with "Live Prototype" badge
3. **Persona Compass**: 6 persona cards (2 Active, 2 Hesitant, 1 Resister color-coded), themes section, What Now callout
4. **Workflows / BoodleBox**: Two-column layout with feature bullets + browser mockup showing Chat UI, shared rooms, active model tags
5. **About**: 3 value props (01/02/03 numbered cards), 5 offering cards, distinction banner
6. **Accelerator banner**: Navy bg, teal accent, rotator text cycling through 5 messages
7. **Use Cases**: Filter buttons (All/MBA/Law/MPA), 8 cards with "Try asking" prompt boxes
8. **Responsible AI**: Intro with EDUCAUSE + AIAS references, 4-lens grid, Do/Don't columns, 8 classroom strategy cards with unique accent colors, 3 policy links
9. **Timeline**: 16 entries with teal gradient line, alternating standard/highlighted dot style
10. **CTA**: Navy bg, two buttons (BoodleBox login + CAILI learn more)
11. **Footer**: White bg, logo + address + 5 social icons, contact info + 9 quick links, teal copyright bar

## Navigation

- **Top bar**: Logo (picture element with responsive srcset) + 46px search icon + MENU button (font-black text-2xl uppercase)
- **Mega menu**: Right-side drawer (max-w-lg), navy header, CAILI Studio links, UBalt section (4 accordion dropdowns), Schools, 4-colored CTA buttons (teal/yellow/purple/pink), Request Information, MyUBalt, BoodleBox login

## Responsive Breakpoints

- **Desktop (lg)**: 1024px+ — full 3-column grids, 80px gutters
- **Tablet (sm/md)**: 640-1023px — 2-column grids, 40px gutters
- **Mobile**: <640px — 1-column stacks, 20px gutters, 66px header

## Animations

- **Reveal**: IntersectionObserver triggers `.reveal.active` — opacity 0→1 + translateY(20px→0) over 600ms
- **Text rotator**: Banner cycles through 5 messages every 3.5s with 300ms fade

## Research Sources

- UBalt-BoodleBox partnership news article (September 2025)
- CAILI Year One impact report (May 2026)
- "Building Baltimore's AI Future" AI Summit article (May 2026)
- AI-Powered Economics Education at UBalt Merrick (May 2026)
- "Understanding Baltimore's AI Ecosystem" report with Mindgrub (June 2026)
- BoodleBox overview and FAQ pages
- EDUCAUSE AI Ethical Guidelines (June 2025)
- AI Assessment Scale (AIAS) framework (Perkins, Furze, Roe, MacVaugh)
- UBalt Generative AI Guidelines (Office of Academic Affairs)
- UBalt CELTT AI Exploration page
