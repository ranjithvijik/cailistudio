CodeX Prompt: Update the CAILI AI Studio Landing Page

This specification describes how to revise the existing CAILI AI Studio landing page based on the latest feedback.  The goal is to bring the design closer to the aesthetic and polish of superagent.com while emphasizing the University of Baltimore’s identity and mission.  The updated design should be full‑bleed, refined and expressive, with graduate‑level use‑case prompts and a stronger ethics narrative.

Full bleed layout
	•	Remove the fixed container width and margins.  Set --container-width to 100% or remove it entirely and adjust .container so that sections and backgrounds extend to the edges of the viewport.  Content can still be centered within their sections, but backgrounds should cover the entire width.
	•	The top navigation bar, hero section and all panels should span the full width of the browser window.  Avoid unused whitespace at the sides.
	•	Use responsive CSS to ensure that this full‑bleed design works smoothly on large screens as well as mobile devices.

Typography and spacing
	•	Increase the base font size for body text to around 1.1rem and set line-height to at least 1.8 for better readability.
	•	Reduce negative letter-spacing—use 0 or -0.01em—and add more vertical space between paragraphs and sections.  Give headings ample breathing room above and below.
	•	Scale up heading sizes slightly (e.g. increase clamp values by 0.2–0.4rem) and lighten the letter spacing on headings for a more airy feel.

Personalised tone and UBalt elements
	•	Incorporate more of the University of Baltimore’s identity.  Display the UBalt crest or tagline in the header and adjust copy throughout the page to reference the University explicitly.  For example: “A campus AI adoption accelerator for the University of Baltimore’s Merrick School of Business, School of Law and Master of Public Administration programs.”
	•	Use language that speaks to students and faculty directly, emphasising community, collaboration and real‑world impact.
	•	Keep CAILI’s mission front and centre.  The hero paragraph should mention that CAILI’s goal is to equip faculty, students and the Baltimore community to responsibly engage with generative AI through ethical, equitable and interdisciplinary learning and research ￼.

Scroll animations
	•	Add a lightweight JavaScript snippet that uses the IntersectionObserver API to detect when each section enters the viewport.  When at least 20% of a section is visible, add a class like .in-view to that section.
	•	In the CSS, define a fade‑in and slight slide‑up animation for elements inside .in-view sections.  Set opacity: 0 and transform: translateY(2rem) initially and transition to full opacity and zero translation over 400–600 ms.
	•	Apply these animations to main sections (hero copy, feature panels, adoption banner, value cards, use cases, ethics, CTA) so they animate into view as the user scrolls down the page.

Highlight cards enhancements
	•	Increase padding and border radius for the four highlight cards in the hero section; add a soft pastel background or gradient to each card and apply a gentle drop shadow (box-shadow with 0 1rem 2rem var(--color-shadow)).
	•	Add a unique icon to each card.  Use Font Awesome or similar icons (e.g. scales for ethics, lightbulb for adoption, layers for discipline workflows, and users for community).  Place the icon at the start of each card.
	•	Increase font size for the card headings and separate them from the card body with a subtle margin.

Revised highlight card content
	1.	Ethical AI in Your Discipline — Focus on fairness, equity, transparency and academic integrity; explain that CAILI’s mission is to equip faculty, students and the Baltimore community to engage responsibly with AI ￼.
	2.	Practical AI Adoption — Highlight how CAILI AI Studio provides guided workflows, curated tools and tailored prompts to streamline research, writing and analysis.
	3.	Discipline‑Specific Workflows — Point out that MBA, School of Law and MPA use cases are built into the platform to help users get started quickly.
	4.	Community & Collaboration — Emphasise BoodleBox integration and collaborative features that encourage shared learning and collective intelligence.

Use‑case section updates
	•	Change the filter label “Law” to “School of Law”.
	•	Add a new filter label “MPA” for the Master of Public Administration program.
	•	For the MPA category, include at least three cards:
	•	Policy Research & Legislative Analysis — Use AI to analyse and summarise legislative proposals, policy documents and stakeholder perspectives.  Example prompt: “Summarise the key provisions of the Maryland Sustainable Communities Act of 2025 and identify potential impacts on Baltimore’s economic development and social equity.”
	•	Grant Writing & Funding Research — Use AI to identify funding opportunities and generate grant proposals.  Example prompt: “Draft a grant proposal outline for a public health initiative aimed at reducing food insecurity in West Baltimore, including a situational analysis, objectives and evaluation metrics.”
	•	Community Needs Assessment & Program Evaluation — Use AI to compile demographic and socio‑economic data and evaluate program effectiveness.  Example prompt: “Compile and summarise the most recent demographic and socioeconomic data for the West Baltimore community and identify key challenges and opportunities for local nonprofit organisations.”
	•	Revise the existing MBA and School of Law cards with stronger, graduate‑level prompts:
	•	MBA – Market Research & Competitive Analysis: “Conduct a competitive analysis of mid‑sized Maryland renewable energy startups, highlighting the top five players, their market strategies, growth trajectories and opportunities for differentiation.  Provide charts and credible citations.”
	•	MBA – Business Writing & Case Analysis: “Compose a strategic analysis of XYZ Corp’s decision to adopt generative AI for product development, including benefits, risks, market positioning and recommendation.”
	•	MBA – Idea Validation & Venture Testing: “Generate a detailed validation plan for a digital mental health platform designed for college students, covering market potential, user personas, revenue models and risk assessment.”
	•	School of Law – Case Law Research & Summarisation: “Summarise three landmark Maryland appellate decisions on freedom of speech in public schools and explain how these precedents apply to the case of Smith v. UBalt.”
	•	School of Law – Drafting Motions & Briefs: “Draft a motion for summary judgment in a hypothetical case involving a negligence claim against a local nonprofit.  Include relevant case law, statutory citations and legal arguments.”
	•	School of Law – Statutory Analysis & Interpretation: “Analyse the Maryland Consumer Protection Act and outline the key elements that must be proved in a deceptive trade practice claim, with examples of how courts have applied the statute.”

Ethics section enhancements
	•	Expand the ethics section into four cards, each covering one of CAILI’s core ethical principles:
	1.	Fairness & Equity — Describe how users should leverage AI to ensure diverse perspectives and avoid biases.  Use a pastel green background.
	2.	Transparency — Encourage users to cite sources and disclose when AI has assisted their work.  Use a pastel blue background.
	3.	Academic Integrity — Explain that AI should support learning and idea development, but that users must produce their own analyses and writing.  Use a pastel yellow background.
	4.	Community Engagement — Highlight how AI can be used to tackle real‑world problems in partnership with the Baltimore community, emphasising CAILI’s mission of social mobility and impact ￼.  Use a pastel pink background.
	•	Provide a “Do’s and Don’ts” list under these cards that clarifies appropriate vs. inappropriate AI use in academic settings.

Call‑to‑action section
	•	Replace the heading “Ready to start your AI journey?” with “Enrich Your Academic Journey with CAILI AI Studio”.
	•	Revise the subheading to: “Discover how AI can enhance your research, writing and learning across UBalt’s MBA, School of Law and MPA programs.”
	•	Leave the buttons as “Log in with BoodleBox” and “Learn more about CAILI”, but ensure they are styled consistently with the new design.  The primary button should use a gradient fill and the secondary button should have a subtle border.

Technical & styling updates
	•	Set .container { width: 100%; margin: 0; padding: 0; } and remove any max‑width limits to achieve a full‑bleed look.
	•	Increase the size of the University of Baltimore and BoodleBox logos in the header and ensure they remain responsive on small screens.
	•	Use consistent pastel backgrounds for the hero highlight cards and ethics cards; adjust the --color-bg-strong and related variables to soften the overall palette.
	•	Implement subtle pastel gradients in the adoption banner and CTA card backgrounds.
	•	Ensure that the filter buttons for “All”, “MBA”, “School of Law” and “MPA” clearly indicate which category is selected by changing background colour and text colour.

⸻

This updated specification should guide CodeX to generate a refined version of the CAILI AI Studio landing page.  It addresses the full‑bleed layout, improves typography, personalises the tone, adds scroll animations, enhances the hero highlights, updates the use‑case categories and prompts, revitalises the ethics section, and refines the call‑to‑action, all while maintaining CAILI’s mission at its core.