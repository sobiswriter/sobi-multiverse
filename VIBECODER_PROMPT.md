# Build Brief: Sobi's Multiverse Portfolio MVP

You are implementing the first MVP of a new portfolio called **Sobi's Multiverse**.

Before touching code, read:

- `docs/plan.md`
- `docs/design.md`
- `docs/architecture.md`
- `docs/rules.md`
- `docs/memory.md`

## Mission

Build the complete portfolio skeleton first.

Do NOT build the final multiverse backgrounds or cinematic universe transitions yet.

The goal of this milestone is a polished, real-content, responsive portfolio application whose architecture is ready for the later visual transformation.

## Required Stack

Use:
- Next.js App Router
- TypeScript
- React
- Tailwind CSS or an equivalent lightweight styling approach
- GSAP for the motion foundation
- React Bits selectively

Do not add additional heavy technologies unless there is a concrete reason.

## Required Sections

Implement these eight sections in this order:

1. Arrival / Home
2. The Builder / Projects
3. The AI Lab / Experiments
4. The Research Room
5. The Arsenal / Skills
6. The Journey / Timeline
7. The Person Behind the Code / About
8. Contact / Beyond

Treat them as future universe IDs `00` through `07`.

## Required Implementation

Create typed data collections for:
- projects
- experiments
- research
- skills
- timeline
- profile
- links
- universe configuration

Create reusable components for:
- global navigation
- section/universe shell
- project cards or project list
- metadata/tags
- buttons/links
- transition overlay
- motion utilities

Use real portfolio information where verified. Do not invent missing information. Anything uncertain should be marked for review.

## Navigation

Implement:
- persistent navigation
- active section state
- next/previous section controls where appropriate
- keyboard navigation
- Escape behavior for overlays
- normal browser navigation behavior

The navigation implementation should already be compatible with future GSAP transition choreography.

## Motion

Use only restrained motion in MVP:
- initial page reveal
- text/item entrance
- subtle hover/focus states
- section reveal
- basic transition overlay hook

Do NOT create the final multiverse travel effect yet.

## Visual Direction

Dark cinematic shell.

Strong typography.

Excellent spacing.

Minimal UI chrome.

No generic SaaS dashboard appearance.

No excessive glass cards.

No random decorative gradients or blobs.

The MVP should look intentionally designed even before the dramatic visual worlds arrive.

## Responsive / Accessibility

Support desktop, tablet, and mobile.

Respect `prefers-reduced-motion`.

All meaningful information must remain accessible without hover.

Use semantic markup and visible focus styles.

## Performance

Optimize and lazy-load images.

Do not ship heavy 3D/WebGL systems in the MVP.

Keep dependencies minimal.

## Deliverables

When finished:

1. Run type checking.
2. Run linting.
3. Run production build.
4. Confirm there are no runtime console errors.
5. Test desktop and mobile layouts.
6. Test keyboard navigation.
7. Update `docs/memory.md` with the final state, bugs, and exact next step.

## Important

Do not stop after creating empty routes.

The sections must contain the actual portfolio information architecture and meaningful content placeholders/data structures so the next phase can focus almost entirely on turning each section into a distinct universe.

Do not redesign the scope midway. Finish the MVP skeleton first.
