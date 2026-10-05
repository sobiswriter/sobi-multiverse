# Sobi's Multiverse Portfolio - Master Plan

## 1. Vision

Build a personal portfolio that behaves like an explorable multiverse rather than a conventional developer website.

The final experience should communicate:

- Sobi builds software, AI systems, experiments, and creative work.
- Sobi thinks in systems and connections, not isolated projects.
- The portfolio itself is evidence of technical range, design taste, and engineering ability.
- Every major section can eventually become its own visual universe with a distinct atmosphere.
- GSAP should choreograph travel between universes while React/Next.js provides the application structure.
- React Bits and other component libraries are raw material, not visual identity by themselves.

## 2. MVP Goal

Before building the multiverse effects, create a complete, production-ready portfolio skeleton with real content, reliable navigation, responsive behavior, and a data-driven architecture.

The MVP should feel intentionally designed even without the final universe effects.

## 3. MVP Information Architecture

Use eight primary sections. These can initially be sections/routes in a straightforward layout and later become eight distinct universes.

### Universe 00: Arrival / Home
Purpose: immediate identity and entry point.

Content:
- Name: Sobi
- Primary positioning statement
- Short one-line description
- Current focus / current status
- Primary CTA: Explore the Multiverse
- Secondary CTA: Resume / GitHub / LinkedIn
- Very subtle preview of the universe system

### Universe 01: The Builder / Projects
Purpose: show strongest shipped work.

Content model:
- Project title
- Short description
- Problem
- What was built
- Technology
- Status
- Links
- Hero/cover image
- Optional metrics/results

Seed this section from the current portfolio and verify every claim before publication. Known project examples include Wat-EWrite, LegalLM, Project AIC, PersonaVerse, AI Overlay, EquityEcho, Cosmos Anomaly, and RIGHT.LEFT.

Do not force every old project into the first visual presentation. The MVP can contain a larger project dataset while highlighting 5-8 flagship projects.

### Universe 02: The AI Lab / Experiments
Purpose: show curiosity and technical experimentation.

Content:
- Small AI prototypes
- Model experiments
- Agent experiments
- Creative coding
- Tooling experiments
- Interesting failures / lessons learned

Each entry should be concise and honest. Prefer "what I tried / what happened / what I learned" over marketing copy.

### Universe 03: The Research Room
Purpose: communicate deeper technical thinking.

Content:
- Research projects
- Computer vision / ML work
- Interesting technical investigations
- Hackathon or ideathon problem-solving
- Research notes
- Technical writeups where available

This section should not pretend everything is academic research. Clearly distinguish research, experimentation, and product work.

### Universe 04: The Arsenal / Skills
Purpose: show the technologies and capabilities behind the work.

Organize by capability rather than a giant logo wall:
- Languages
- Frontend
- Backend
- AI / ML
- Developer tooling
- Creative technologies
- Deployment / infrastructure

Use the project data to support skill claims wherever possible.

### Universe 05: The Journey / Timeline
Purpose: show progression and context.

Content:
- Education
- Major builds
- Hackathons / ideathons
- Recognition / awards
- Publications / patents where applicable
- Major technical milestones

Timeline entries should be chronological and factual.

### Universe 06: The Person Behind the Code / About
Purpose: human context.

Content:
- Short biography
- What motivates the work
- Interests
- How Sobi approaches building
- Current direction
- Optional portrait

Keep this section concise. The portfolio should reveal personality through the entire experience rather than dump autobiography into one page.

### Universe 07: Contact / Beyond
Purpose: clear next action.

Content:
- Email
- GitHub
- LinkedIn
- Resume
- Availability / collaboration statement
- Closing line tied to the multiverse concept

The contact experience should be extremely simple even if the visual presentation is elaborate.

## 4. MVP Functional Requirements

### Navigation
- Persistent global navigation.
- Every major section reachable within two interactions.
- Active-section indication.
- Keyboard accessible.
- Escape closes overlays/modals.
- Browser back/forward behavior must remain sensible.

### Content
- All portfolio content stored in structured local data files.
- No important content hard-coded inside presentation components.
- Projects, skills, timeline items, experiments, and links must be independently editable.

### Responsiveness
- Desktop-first creative direction, but fully usable on tablet and mobile.
- Motion must degrade gracefully on low-power devices.
- Touch interactions must never depend on hover.

### Accessibility
- Semantic HTML.
- Keyboard navigation.
- Visible focus states.
- Sufficient contrast.
- Reduced-motion support.
- Images must have meaningful alt text where appropriate.

### Performance
- Optimize images.
- Avoid loading heavy visual effects before they are needed.
- Lazy-load noncritical media.
- Avoid a giant dependency pile just because a component looks interesting.
- Maintain good Core Web Vitals.

## 5. MVP Visual Direction

The MVP should use a neutral visual shell so the later universe-specific visual systems can be swapped in without rebuilding the content architecture.

Base direction:
- Dark, cinematic foundation.
- Strong typography hierarchy.
- High-quality spacing.
- Restrained UI chrome.
- Subtle motion only.
- No final universe-specific background effects yet.

The shell should already contain the hooks/components needed for future transitions:
- Universe container
- Transition overlay
- Page/section transition controller
- Global cursor layer
- Scroll progress/state
- Reduced-motion state

## 6. MVP Deliverables

The vibecoder is done with MVP when all of these exist:

1. A working Next.js + TypeScript portfolio application.
2. Eight complete sections using real, editable content.
3. Responsive layouts for desktop/tablet/mobile.
4. Data-driven project, skill, timeline, and experiment collections.
5. Persistent navigation and working internal links.
6. Resume/GitHub/LinkedIn/contact links wired correctly.
7. Initial GSAP foundation installed and used sparingly for shell-level motion.
8. React Bits/components integrated only where they fit the design system.
9. Reduced-motion and accessibility support.
10. No placeholder lorem ipsum or fake achievements.
11. Documentation files completed: `plan.md`, `design.md`, `architecture.md`, `rules.md`, `memory.md`.
12. README with local setup, scripts, architecture overview, and content-editing instructions.

## 7. Post-MVP Roadmap

### Phase A: Foundation
Finish the MVP above.

### Phase B: Universe Identity
Give each section a completely different art direction, background system, typography treatment, interaction language, and ambient motion.

### Phase C: Inter-Universe Travel
Build cinematic GSAP transitions between sections. The transition itself becomes a reusable system.

### Phase D: Interactive Worlds
Turn selected project entries into explorable micro-experiences rather than static cards.

### Phase E: Advanced Visual Layer
Evaluate WebGL/Three.js/shaders/R3F only where they provide meaningful value.

### Phase F: Hidden Layer
Add optional easter eggs, secret routes, experimental interactions, and deeper portfolio lore without making the main UX confusing.

## 8. Definition of Success

The final portfolio should make a visitor remember the experience and the person behind it.

A strong visitor reaction is not merely:

"Nice portfolio."

It is:

"I have never seen a portfolio work like that before."

The site must still communicate competence clearly within the first minute. Spectacle is the delivery mechanism, not the substitute for information.
