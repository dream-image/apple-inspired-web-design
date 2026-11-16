---
name: apple-inspired-web-design
description: Design and implement Apple-inspired desktop websites, mobile app-style web interfaces, H5/PWA, and Electron UIs from requirements, content, or existing screens. Adapt to the existing React, Vue, or other web stack. Use for Apple-style web generation or redesign, not native SwiftUI development or review-only auditing.
---

# Apple-inspired Web Design

Turn real content, tasks, and brand identity into clear, restrained, polished, usable web interfaces. Do not reduce Apple-inspired design to white backgrounds, oversized corners, or blur everywhere. This is an original web implementation workflow, not an official Apple component system, certification, or copy of private implementation.

## Boundaries

- Interpret “app” as an app-like mobile web interface/H5/PWA unless the user explicitly requests native or hybrid engineering.
- For design requests, deliver an implementable specification. For generation/redesign requests, deliver working code, not just a review. Preserve business behavior, APIs, routing, and the existing stack; do not migrate frameworks without authorization.
- Follow the project's AGENTS.md, component library, and brand constraints. Invoking this skill does not authorize dependency installation, real payments, publishing, or unrelated global configuration changes.
- Read [sources-and-principles.md](references/sources-and-principles.md) for provenance. Verify current official documentation for Apple-specific platform rules or APIs. Do not translate native points, system menus, or gestures directly into mandatory web rules.

## 1. Let content determine the interface

Read the supplied material and relevant project context. Identify audience, primary task, content types, key actions, existing states, and constraints. Infer reasonable defaults; ask only about missing facts that would materially change the product direction.

Briefly establish these design decisions:
- Who is this page for, what does it help them do, and what is its primary action?
- What is the information hierarchy? Do not start with a generic hero-and-three-cards template.
- Is this a product workspace or a presentation page? Tools, administration, and editors prioritize efficiency. Large display headlines, visual storytelling, and expansive spacing belong where the content warrants them.
- Choose one product-relevant distinguishing element; let surrounding elements recede. A deliberately quiet utility is a valid direction.
- Explain how desktop and mobile organize navigation and accomplish the same task.

Use clearly labeled demonstration data when necessary. Never invent testimonials, business metrics, partner brands, or working backend capabilities.

## 2. Define the visual system before generating components

Read [web-patterns.md](references/web-patterns.md) before layout. Reuse existing tokens; otherwise define semantic colors, typography roles, spacing, radii, elevation, and motion. All suggested numbers are adjustable web starting points, not official Apple pixel specifications.

- Express hierarchy through content, size, weight, spacing, and grouping. Navigation, body text, secondary information, and primary actions need clear ordering.
- Prefer system fonts and verify actual Chinese fallback fonts and line heights. Do not download or bundle Apple-specific fonts or symbol assets to imitate a native app.
- Use one primary accent and stable semantic state colors. Avoid full-screen saturated gradients, stacked shadows, or decorative numbers.
- Apply coherent radii by control/container/overlay level. Do not give every element the same oversized corner; lists and prose need not become cards.
- Glass is optional functional-layer treatment, preferably limited to a few floating navigation or toolbar surfaces. Keep content legible and stable. Material cannot replace information architecture.
- Prefer familiar, accessible HTML or existing component primitives; adapt their styling rather than reinventing basic interactions.

## 3. Design desktop and mobile task paths together

Do not merely shrink desktop layouts. Reorganize by available space while preserving tasks, data, filters, and editing context.

- Desktop: allow sidebars, master-detail panes, appropriate density, quick actions, and keyboard paths. Do not draw fake macOS window controls or system menus in ordinary web pages.
- Mobile: favor one column and reachable primary actions. Use bottom navigation or sheets when justified, not universally. Navigation changes destinations; action buttons perform tasks.
- For tables, choose horizontal scrolling, column priority, or summary lists according to the task. Preserve essential fields and actions. Collapsed toolbars must retain discoverable functionality.
- Use fluid widths, minmax, clamp, and content-driven breakpoints. Handle safe areas, virtual keyboards, browser navigation, and long content. Do not lock the entire page height or disable zoom.

## 4. Implement complete states and real interactions

Cover the default, hover, focus, pressed, disabled, loading, empty, error, and success states relevant to the task. Do not build a state system for unrelated features.

- Every interactive element needs real behavior or an explicit demonstration limitation. Use the existing data layer; never fake persistence with a success toast.
- Important changes should be cancellable or recoverable where possible; explain irreversible consequences. Preserve entered data and provide actionable recovery after errors.
- Dialogs need appropriate focus entry, containment, restoration, and dismissal. Prefer established accessible implementations for complex controls. Mobile operation must not depend exclusively on hover or gestures.
- Motion explains relationships and gives feedback without delaying frequent work. Respect reduced-motion. Do not default to WebGL, scroll hijacking, or perpetual bouncing for a “premium” feel.
- Use semantic tokens for light/dark appearances. Follow system preferences while preserving existing user appearance controls. Do not import a third-party skill's native “no in-app theme switch” rule into the web.

## 5. Run, inspect, and refine

Use [verification.md](references/verification.md). Verify real tasks before visual polish. When execution is available, inspect the rendered desktop and mobile pages, fix visible defects, and recheck. When unavailable, disclose the limitation; compilation is not visual validation.

Report implementation locations, key design decisions, actual viewport and interaction checks, and remaining unverified areas. For design-only work, deliver desktop/mobile layout specifications, tokens, and state behavior. For code requests, do not substitute a long guideline report for usable code.

## Example requests

- “Use $apple-inspired-web-design to generate a React order-management interface from these requirements, usable on desktop and phone.”
- “Redesign this Vue settings page with this skill, preserve the APIs, and favor restrained macOS-like clarity without Liquid Glass.”
- “Design a product website from this copy, Apple-inspired but retaining our brand; first provide desktop and mobile directions.”
