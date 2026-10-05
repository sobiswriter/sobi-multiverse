# Rules for AI Agents and Vibecoders

These rules are mandatory for any agent working on Sobi's Multiverse.

## 1. Protect the Concept

This is not a generic developer portfolio.

Do not flatten the site into:
- hero
- cards
- skill logos
- generic contact form

The architecture may be conventional. The experience should not be.

## 2. Do Not Invent Facts

Never fabricate:
- projects
- metrics
- awards
- clients
- employment
- publications
- skills
- dates
- links

When information is unknown, mark it as TODO or ask for the missing information.

## 3. Content First

Do not spend hours polishing an animation around missing content.

Complete the information architecture and content model before building elaborate effects.

## 4. Do Not Over-Engineer the MVP

No unnecessary backend.

No database unless a requirement genuinely appears.

No authentication.

No CMS unless requested.

The first release is primarily a static/content-driven application.

## 5. Keep Data Separate

Do not bury portfolio content inside JSX.

Editable information belongs in typed content/config files.

## 6. Motion Has a Purpose

Every major animation should communicate:
- location
- hierarchy
- state
- causality
- transition
- interaction feedback

Never add motion only because a library makes it easy.

## 7. Respect Reduced Motion

Every significant animation needs a reduced-motion path.

## 8. Mobile Is a First-Class Experience

Do not copy desktop interactions blindly to touch screens.

Hover is optional.
Information is not.

## 9. Accessibility Is Not Optional

Use semantic HTML, keyboard navigation, focus management, meaningful labels, and visible focus states.

## 10. Dependency Discipline

Before adding a package:

1. Check whether the same result can be achieved with existing dependencies.
2. Check bundle/performance cost.
3. Check maintenance quality.
4. Check whether the library actually fits the visual system.

## 11. Do Not Rewrite Working Systems Without Cause

Make the smallest coherent change that solves the problem.

Preserve existing behavior unless the task explicitly changes it.

## 12. Test After Meaningful Changes

At minimum verify:
- build passes
- TypeScript passes
- no console errors
- navigation works
- responsive layout works
- animations clean up correctly

## 13. Keep Documentation Current

When architecture changes, update `architecture.md`.

When design rules change, update `design.md`.

When implementation state changes materially, update `memory.md`.

When the overall goal changes, update `plan.md`.

## 14. Agent Handoff Rule

Never assume previous chat context exists.

At the start of a work session:
1. Read `memory.md`.
2. Read `plan.md` for current goals.
3. Read `architecture.md` before structural changes.
4. Read `design.md` before visual changes.
5. Read `rules.md` before writing code.

At the end of a substantial session, update `memory.md` with only durable project state.
