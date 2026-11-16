# Apple-inspired Web Design

An independent agent skill for designing and implementing Apple-inspired desktop websites, mobile app-style web interfaces, H5/PWA, and Electron UIs from real content and requirements.

## What it does

- Turns content and user tasks into information hierarchy and implementable interfaces.
- Adapts to existing React, Vue, and other web stacks without imposing a component library.
- Designs desktop and mobile task paths together.
- Covers semantic design tokens, accessible interactions, restrained glass/motion, realistic states, and browser verification.
- Distinguishes official design principles from original web implementation advice.

## Use

Copy this directory into your agent's skills directory under `apple-inspired-web-design`. For Codex, a typical user-level location is `~/.codex/skills/apple-inspired-web-design`.

Then ask:

> Use $apple-inspired-web-design to implement this order-management interface for desktop and phone, preserving our existing stack and APIs.

For design-only work, explicitly request a specification before implementation.

## Contents

- `SKILL.md`: trigger, boundaries, and generation workflow.
- `references/sources-and-principles.md`: sources and original web adaptations.
- `references/web-patterns.md`: web implementation suggestions.
- `references/verification.md`: responsive, interaction, accessibility, and engineering checks.

## Sources and status

Inspired by [Apple's design principles](https://developer.apple.com/cn/design/human-interface-guidelines/design-principles) and the review methodology of [dickwu/apple-design-skill](https://github.com/dickwu/apple-design-skill). References were reviewed on 2026-11-16. This repository contains original workflow guidance, not a mirror of Apple's documentation or the other skill's reference collection.

This is not an Apple product, official component library, certification, or guarantee of HIG compliance or App Store approval. Native platform rules must be verified against current official documentation rather than mechanically applied to the web.

Structural checks have passed. The skill has not yet undergone forward-testing on a real application. Suggested sizes and animation timings are adjustable web starting points, not official Apple specifications.
