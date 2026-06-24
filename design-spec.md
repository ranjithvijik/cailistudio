CodeX Prompt: Build the CAILI AI Studio Landing Page

Your task is to create a modern, responsive landing page for “CAILI AI Studio,” inspired by the design of superagent.com.  The site will serve as a campus AI adoption accelerator for the University of Baltimore’s Merrick School of Business while signalling its applicability to the School of Law and other programmes.  Your code must be original; do not copy any source from superagent.com.  Instead, implement similar styling and layout using HTML, CSS and, where necessary, JavaScript.

Design resources and assets

In addition to the instructions below, you will have access to a Design folder in the project root containing sample pages and assets.  Before you begin writing code, open the files in this folder (for example, a full landing page and a use‑cases page) to understand how colour, spacing and typography are used.  You may reference these pages for inspiration, but do not copy their markup or styles verbatim.  Use them to inform your own layout and styling decisions.

This folder will also include official logos and images for the University of Baltimore and BoodleBox, along with illustrative graphics for the feature panels.  When implementing the design:
	•	Replace the header’s left‑side placeholder with the actual University of Baltimore logo from the Design folder.  Provide appropriate alt text (e.g., alt="University of Baltimore logo") for accessibility.
	•	In the BoodleBox integration panel, include the BoodleBox logo and an image representative of the BoodleBox interface.  Use the logo provided in the assets folder and add descriptive alt text (e.g., alt="BoodleBox logo").
	•	For the right panels of feature sections, instead of generic placeholders, use the supplied panel images (e.g., charts, dashboard mock‑ups) found in the assets directory.  These images should be inserted as <img> tags within your stylised browser mock‑ups and scaled appropriately to maintain aspect ratio.
	•	All images must be responsive.  Set max-width: 100% and height auto so they scale gracefully on smaller screens.

Finally, include HTML comments in your code specifying where the logos and images came from (e.g., <!-- University of Baltimore logo from /Design/assets/ub_logo.svg -->).  This helps other developers understand the asset origins.

General guidelines
	•	Colour scheme: Use a soft beige or cream (#F9F5EB or similar) as the base colour across the page.  Employ a gradient accent—purple fading to pink (e.g. #5E2CA5 → #C94FC4)—for highlighted text, buttons and other accents.  Use black for primary text and dark gray for secondary descriptions.  Define these as CSS variables.
	•	Typography: Set a global sans‑serif typeface such as Inter, Helvetica or a similar free font.  Headings should be bold and large; body text should be regular weight.  Apply letter‑spacing and generous line‑height to enhance readability.
	•	Layout: Emphasise generous whitespace.  Use flexbox or CSS Grid to organise content into rows and columns that adapt to different screen sizes.  Cards and panels should have rounded corners and subtle drop shadows.  Ensure the layout is mobile responsive; on small screens, stack columns vertically.
	•	Accessibility: Use semantic HTML5 elements (<header>, <nav>, <section>, <article>, <footer>).  Provide ARIA labels for navigation and interactive elements.  All buttons and links should have descriptive text for screen readers.

Page structure

Header
	•	Create a sticky <header> across the top of the page.  Divide it into two horizontal sections.
	•	Left side: Insert a placeholder image or SVG for the University of Baltimore logo and place the text “University of Baltimore” next to it.  This replaces the “Think deeper.” branding used on superagent.com.
	•	When using the real logo from the Design folder, ensure it is aligned vertically with the text and constrained in height (e.g., 40 px).  Use CSS flexbox to align the logo and text.
	•	Right side: Include a plain “Log in” link and a prominent “Sign Up” button styled with a dark background and white text.  Use padding and border‑radius to achieve a pill‑shaped button.  Ensure the header remains visible on scroll.

Hero section
	•	Immediately below the header, create a full‑width hero <section> with a soft beige background.
	•	Add a large heading that reads “CAILI AI Studio.”  To emulate the superagent hero, apply the gradient accent to part of the text; for example, colour “CAILI AI” in black and “Studio” in the purple‑to‑pink gradient.  Use a bold, oversized font.
	•	Under the heading, write a short paragraph that not only describes the platform’s purpose but also highlights CAILI’s mission.  The mission, according to UBalt, is to “equip faculty, students, and the Baltimore community to responsibly engage with generative AI through ethical, equitable, and interdisciplinary learning, research, and innovation”—a mission that fosters AI fluency, drives social mobility, and applies technology to solve real‑world challenges ￼.  For example: “Your campus portal for responsible AI adoption and community‑engaged innovation.  Our mission is to equip faculty, students and the Baltimore community to responsibly engage with generative AI through ethical, equitable and interdisciplinary learning and research, driving AI fluency, social mobility and real‑world problem solving.”  Centre this text and limit the width for readability.
	•	Place a primary call‑to‑action button labelled “Log in with BoodleBox” below the paragraph.  Style it with the gradient accent and rounded corners.  For the prototype, set the button’s href to https://boodlebox.ai/ so that it redirects users to the official BoodleBox site.  You can refine this integration later when a dedicated UBalt login route is available.  Optionally include a secondary button for “Learn more about CAILI.”
	•	Place an additional line of text or a badge near the call‑to‑action that emphasises that BoodleBox access is included for all students and faculty (e.g., “Free & Unlimited through UBalt”).  This reinforces the partnership and invites users to explore BoodleBox as part of their institutional privileges.

Feature sections

Replicate the two‑column panel layout of superagent’s “Super Reports” and “Super Slides” sections, but tailor the content to CAILI’s mission.
	1.	MBA AI Workflows
	•	Use a <section> with a light card background and subtle border.  Create two <div>s inside: left for text, right for an image placeholder.
	•	Left panel:
	•	Heading: “MBA AI Workflows.”
	•	Paragraph describing how CAILI AI Studio guides MBA students through common business tasks.  Example: “Structured AI workflows for market research, business writing and idea validation.”
	•	List three bullet points.  Each bullet can start with a small icon (use Font Awesome) and a bolded feature name followed by a short description.  Suggested bullets:
	•	Data‑driven market research – surface credible data and insights for competitive analysis.
	•	Automated business writing – generate drafts for case analyses, essays and business plans.
	•	Structured idea validation – prompt frameworks to vet new product or service ideas.
	•	Right panel: Create a stylised browser mock‑up using a rounded rectangle with a header bar.  Inside, insert a placeholder graphic or a screenshot of a report.  Maintain a 16:9 aspect ratio to echo superagent’s design.
	2.	BoodleBox Integration
	•	In the second panel, describe how CAILI AI Studio integrates with BoodleBox.  Title the panel “BoodleBox Integration.”  Make clear that for now the “Log in with BoodleBox” button links to the BoodleBox homepage (https://boodlebox.ai/).  Note that deeper integrations—such as single sign‑on or dedicated course bots—can be added in future versions.
	•	Include text explaining that BoodleBox provides free, unlimited access to enterprise‑grade AI models for all UBalt students and faculty ￼, and that CAILI AI Studio serves as the gateway.  Suggested bullets:
	•	One‑click access to multiple models – access GPT‑4, Claude, Gemini and others through a single login ￼.
	•	Collaborative class projects – use BoodleBox’s shared workspace features with transparency and citation support ￼.
	•	Academic success tools – leverage study guides, research assistants and concept explanations ￼.
	•	Use a similar two‑column layout with a browser mock‑up on the right displaying an example of a BoodleBox chat or dashboard.
	•	Replace the placeholder in the mock‑up with the actual BoodleBox interface graphic from the Design assets folder.  If none is available, create a simple wireframe using nested <div> elements to suggest chat bubbles or dashboard panels.

Adoption accelerator banner
	•	Implement a colourful horizontal banner to capture attention, inspired by the pastel slider from superagent’s home page.  This can be a full‑width <div> with a pastel background (choose from pink, peach or lavender) and large rounded corners.
	•	Centre a bold statement within the banner, such as: “Accelerate Your AI Adoption.”  Underneath, add a subheading: “Unlock responsible AI literacy across the Merrick School of Business and beyond.”  Use a button on the right side labelled “Get Started” and style it with the accent gradient.  On mobile, stack the button below the text.
	•	Consider animating or cycling through brief taglines or statistics in a subtle way (e.g., fade in/out) to highlight adoption metrics or success stories from MBA students.  Use CSS transitions; avoid heavy JavaScript.
	•	Optionally include a small label (such as “Researching…” or an icon) above the statement to evoke a dynamic feel.

Value proposition section
	•	Create a new section with a heading split across two lines: “Accelerate adoption.” on the first line and “Empower learning.” on the second line.  Apply the gradient accent to the second line to mirror the “Exhaustive research. Expressive results.” treatment ￼.
	•	Beneath the heading, arrange three equal‑width cards horizontally (stack vertically on small screens).  Each card should have a light background, rounded corners and a slight shadow.
	1.	Guided Workflows – Describe how the studio provides structured tasks, prompts and templates that map to common MBA and law school assignments.
	2.	BoodleBox Access – Explain that the platform delivers free, unlimited access to enterprise‑grade AI models and academic success tools ￼ ￼, encouraging widespread adoption across courses.
	•	Include a note that adoption remains low despite the partnership announced in 2025, and that the CAILI AI Studio’s mission is to drive awareness and support to embed BoodleBox into academic and research workflows.  Encourage both students and faculty to log in and explore their free resources.
	3.	Responsible Use – Emphasise CAILI’s mission to equip faculty, students and the Baltimore community to engage with AI ethically, equitably and interdisciplinarily ￼.  Mention transparency and academic integrity ￼.
	•	Provide a brief description of how these principles can guide usage across disciplines: emphasise fairness in business decision‑making and caution in legal reasoning.  This hints at how the same platform can be adapted for the School of Law and other programmes.

Use‑case grid (optional second page or lower section)
	•	Add a section titled “What can you build with CAILI AI Studio?” Use the gradient accent on “CAILI AI Studio.”  Below the heading, add a short paragraph describing that the AI studio handles the heavy lifting so students can focus on decision making.
	•	Implement pill‑shaped filter buttons for “All,” “MBA” and “Law.”  The active button should have a dark background; inactive buttons should use an outline style.
	•	Display a responsive grid of cards (three per row on desktop).  Each card should resemble those on superagent’s Use Cases page: light background, rounded corners, subtle border.  For each MBA card, include:
	•	Two small labels in the top left corner (e.g., “MBA” and “Workflow”) styled as small pills with a black background or border.
	•	A bold heading describing the use case (e.g., “Market Research & Competitive Analysis”).
	•	A short description explaining how the AI studio facilitates that task.
	•	A quote box at the bottom with an example prompt that the student might enter.
	•	Use icons or small logos to visually differentiate categories (e.g., MBA vs Law).  Keep each icon within a square of 24 × 24 px and reference relevant assets from the Design folder.
	•	Include both MBA and Law cards in your grid to demonstrate that the platform serves multiple programs.  After the MBA use cases, add at least two sample cards for law students and faculty.  Suggested law workflows include:
	•	Case Law Research & Summarization – synthesise cases and identify relevant precedents, facts, and judicial reasoning to support legal arguments.
	•	Drafting Motions & Briefs – generate structured outlines, citations and draft language for motions, briefs and memos, helping law students organise their thoughts.
	•	Statutory Analysis & Interpretation – summarise statutes, regulations and rules, and suggest relevant interpretations or applications to hypothetical scenarios.
	•	These law cards should follow the same visual style as the MBA cards, with labels (e.g., “Law” and “Workflow”), a bold heading, a concise description, and a quote box featuring an example prompt.  Adjust the filter buttons so users can toggle between “All,” “MBA” and “Law” to display the appropriate cards.
	•	Leave comments in the HTML indicating how additional programmes (e.g., Public Affairs, Arts and Sciences) could be added by replicating this card pattern and supplying relevant use cases.

Ethical framing
	•	Include a separate section titled “Responsible AI & Ethical Guidelines.”  Use a light card background and a subtle border.  Inside, summarise CAILI’s ethical principles:
	•	Promote fairness and equity in AI applications.
	•	Maintain transparency and academic integrity ￼.
	•	Engage the Baltimore community through community‑led innovation ￼.
	•	Encourage thoughtful, ethical and interdisciplinary AI adoption ￼.
	•	Explain that these principles guide all interactions within the AI studio and must be respected when using BoodleBox.
	•	To further emphasise the ethical focus, provide examples of acceptable and unacceptable AI use (e.g., “Use AI to summarise articles and create outlines, but write final analyses in your own words.”).  Include footnotes or links to UBalt’s academic integrity policies.

Call to action & Footer
	•	Finish the page with a full‑width call‑to‑action section.  Use a beige background.  Add a headline such as “Ready to start your AI journey?” and a subheading inviting MBA and law students and faculty to adopt CAILI AI Studio as their AI companion.
	•	Provide two buttons: “Log in with BoodleBox” (using the accent gradient) and “Learn more about CAILI.”  Align the buttons horizontally on desktop and stack them on mobile.
	•	For the footer, replicate the minimalist style of superagent: align the CAILI tagline (“CAILI AI Studio”) to the left; on the right, include a list of simple links (“About”, “Use Cases”, “Contact”, “Terms”, “Privacy”).  End with a copyright notice referencing the University of Baltimore.
	•	Add a small note at the bottom of the footer saying “Design inspired by superagent.com.  All trademarks remain property of their respective owners.”  Include social media icons if desired (use Font Awesome or similar).

Technical requirements
	•	Save the main HTML as index.html and the stylesheet as styles.css in the project root.  Link the CSS file in the <head> of your HTML.
	•	Define CSS variables for colours and fonts at the :root level (e.g., --color-bg, --color-accent-start, --color-accent-end, --color-text, etc.).  Use these variables consistently.
	•	Use CSS Flexbox or Grid to arrange columns.  Ensure the layout collapses gracefully on narrower screens: panels should stack vertically and buttons should expand to full width.
	•	Include comments in the code to indicate where content could be extended or modified for other UBalt schools (e.g., Law).
	•	Use placeholder images for report screenshots and diagrams; these can be plain coloured boxes with labels such as “Report Preview.”
	•	You may add minimal JavaScript to handle filter button interactions in the use‑case grid.  Use unobtrusive script placement or external JS files.

Accessing design references

Prior to coding, open the contents of the Design folder in the project root.  The folder contains sample HTML/CSS files and assets from the University of Baltimore that represent the current design guidelines.  Treat these files as reference only; do not reuse their code directly.  Observe how sections are laid out, how cards are styled, and how images are integrated.  Use this knowledge to inform your implementation of the CAILI AI Studio, ensuring consistency with the institution’s visual identity.  When working with CodeX, you can instruct it to open these files for context by specifying their relative paths (e.g., Design/landing-page.html).

⸻

By following these instructions, your CAILI AI Studio landing page will evoke the polished, modern aesthetic of superagent.com while centring the University of Baltimore’s mission.  It will clearly highlight the BoodleBox integration and encourage adoption across the Merrick School of Business, signalling scalability to the School of Law.  Most importantly, it will foreground CAILI’s commitment to responsible AI literacy and ethical engagement on campus ￼.