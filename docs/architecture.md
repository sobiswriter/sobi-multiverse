# Architecture - Sobi's Multiverse

## Stack

Recommended foundation:
- Next.js (App Router)
- TypeScript
- React
- Tailwind CSS or a small CSS architecture for layout/utilities
- GSAP for motion orchestration
- React Bits for selected interaction primitives
- Lenis only if smooth scrolling is genuinely needed
- Three.js / React Three Fiber only after profiling and only for effects that justify it

## Architectural Principle

Separate content, presentation, motion, and universe configuration.

The goal is to make it possible to redesign a universe without rewriting project data or navigation logic.

## Suggested Structure

```text
app/
  page.tsx
  layout.tsx
  globals.css
  projects/
  experiments/
  research/

components/
  navigation/
  sections/
  projects/
  ui/
  motion/
  universe/

content/
  projects.ts
  experiments.ts
  research.ts
  skills.ts
  timeline.ts
  profile.ts
  links.ts

lib/
  gsap/
  navigation/
  accessibility/
  utils/

config/
  site.ts
  universes.ts

public/
  images/
  projects/
  textures/

/docs/
  plan.md
  design.md
  architecture.md
  rules.md
  memory.md
```

## Content Model

Keep content in typed data collections.

Example project shape:

```ts
export type Project = {
  id: string
  title: string
  slug: string
  summary: string
  description?: string
  role?: string
  technologies: string[]
  category: 'ai' | 'web' | 'research' | 'creative' | 'tooling' | 'game'
  status: 'live' | 'active' | 'archived' | 'prototype'
  featured: boolean
  links: {
    demo?: string
    github?: string
    article?: string
  }
  media?: {
    hero?: string
    gallery?: string[]
  }
}
```

Create equivalent typed models for experiments, research entries, skills, and timeline items.

## Universe Model

Universe configuration should be separate from section content.

Suggested shape:

```ts
export type UniverseConfig = {
  id: string
  label: string
  section: string
  theme: string
  background: 'solid' | 'particles' | 'canvas' | 'shader' | 'scene'
  enterTransition: string
  exitTransition: string
  effectsEnabled: boolean
}
```

The MVP can use the same visual shell for all universes while preserving this configuration boundary.

## Motion Architecture

Create a small motion layer rather than importing GSAP logic everywhere.

Example responsibilities:
- `transitionToUniverse()`
- `enterSection()`
- `leaveSection()`
- `revealText()`
- `staggerItems()`
- `respectReducedMotion()`

GSAP contexts must be scoped to mounted components and cleaned up on unmount.

## Navigation Architecture

One source of truth for the universe order.

Navigation should support:
- direct section navigation
- next/previous universe
- keyboard navigation
- future transition choreography

Avoid duplicated section names across components.

## Performance Architecture

Heavy experiences must be code-split.

A future shader or 3D universe must not make the entire first load expensive.

Load expensive visual layers only when entering the corresponding universe.

## SEO / Metadata

The site must remain indexable despite being experiential.

Each important page/section should have:
- meaningful title
- description
- Open Graph metadata
- semantic headings
- crawlable textual content

Do not hide all portfolio information inside canvas/WebGL.

## Error / Failure Behavior

Visual effects are enhancements.

If GSAP, WebGL, an image, or a third-party component fails, the content and navigation must still work.
