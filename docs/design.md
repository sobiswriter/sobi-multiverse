# Design System - Sobi's Multiverse

## Core Design Principle

The portfolio is one product containing multiple visual realities.

The universes may look radically different, but they must still feel like they belong to the same machine.

The shared identity comes from:
- typography discipline
- interaction quality
- motion choreography
- spacing rhythm
- navigation behavior
- transition language
- quality of copy

## MVP Shell

Until the multiverse phase begins, use a restrained dark shell.

### Typography

Use one display family and one utility/body family at most.

Hierarchy:
- display: identity and major section titles
- heading: project/section titles
- body: descriptions
- mono/utility: metadata, tags, dates, system labels

Do not use novelty fonts merely because they look futuristic.

### Layout

Use a consistent content grid with generous negative space.

Prefer:
- strong compositions
- asymmetry where intentional
- large type
- compact metadata
- deliberate whitespace

Avoid:
- dashboard-like layouts
- excessive rounded cards
- generic glassmorphism everywhere
- random gradients
- decorative blobs with no purpose

## Universe Design Rules

Each universe should eventually define:

1. Atmosphere
2. Dominant visual metaphor
3. Background technology
4. Typography treatment
5. Primary interaction
6. Ambient motion
7. Transition-in behavior
8. Transition-out behavior
9. Accessibility fallback

A universe should feel meaningfully different from the previous universe within 2-3 seconds of entering it.

## Motion Philosophy

Motion should communicate state, hierarchy, geography, or causality.

Good examples:
- entering a project pulls the scene toward it
- changing universe changes environmental motion
- navigation indicates spatial movement
- related projects illuminate through connection

Bad examples:
- perpetual floating for decoration
- exaggerated hover scaling on every object
- animation that delays reading
- scroll hijacking that fights the user

## GSAP Principles

Use timelines and reusable contexts.

Every significant animation should have:
- enter state
- active state
- exit state
- reduced-motion behavior

Avoid dozens of unrelated tweens scattered across components.

## Component Library Use

React Bits components should be adapted to the Sobi visual language.

Do not build the portfolio as a catalogue of React Bits demos.

For each component, ask:
- Does it improve information delivery?
- Does it reinforce the universe concept?
- Can it survive the full design system?

## Responsive Design

Desktop can be theatrical.
Mobile must be editorial and intentional.

Never require a desktop-only interaction to understand a project.

## Accessibility

Respect `prefers-reduced-motion`.

Every interaction that depends on hover needs a touch/keyboard equivalent.

Motion should never be the only way to understand hierarchy.
