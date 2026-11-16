# Web implementation reference

Parameters here are suggested starting points, not Apple specifications, and do not override existing product tokens.

## Tokens and typography

- Semantic colors: canvas, surface, elevated, text, muted, separator, accent, danger, focus. Define light/dark values separately and inspect state combinations.
- Prefer system-ui, -apple-system, BlinkMacSystemFont, and the project's Chinese fallbacks. Start around 14–16px for interface body text and 16px on mobile, then adjust for density and readability. Native points are not CSS pixels.
- Use rem for major type sizes; accommodate Chinese text and line height. Do not make body text tiny and pale for sophistication. Use tabular-nums when comparing numbers.
- A limited spacing sequence such as 4/8/12/16/24/32/48px is a useful start. Keep related controls consistent without forcing all content onto a rigid grid.
- Try 8–12px control radii and 16–24px panel radii; reserve capsules for meaningful buttons/tags. Nested radii should look coherent.
- Shadows express elevation; separators express relationships. Brand can live in imagery, copy, and one characteristic composition, not imitation Apple logos or product marks.

## Content determines components

- Frequent selection: segmented controls for a few choices, selects/searchable selectors for larger sets. Do not conflate navigation and filtering.
- Settings: group labels, descriptions, and controls. Separate dangerous operations; clarify defaults and save timing.
- Workspaces: expose important tasks, filters, and results first. Do not force marketing heroes or meaningless KPI cards into them.
- Content presentation: prioritize reading width, image proportions, and continuous hierarchy. Display headlines must not crowd out content.
- Desktop master-detail can become list-to-detail on mobile. Restore selection, scrolling, and filters on return.
- Put field errors beside fields and retain data after failed submission. Prevent duplicate real requests without leaving loading permanently locked.

## Material and motion

Default to opaque surfaces. If using glass, limit its region and maintain stable legibility against underlying content. Check @supports fallbacks, light/dark backgrounds, scrolling, and mobile performance around backdrop-filter. SVG refraction/WebGL are optional, not requirements; blur support does not establish complex-refraction compatibility.

Try 120–200ms for lightweight feedback and 200–320ms for panel transitions; keep displacement small and favor transform/opacity. Restrained springs are acceptable; inputs, tables, and repeated actions should not bounce continually. Under prefers-reduced-motion, remove nonessential displacement/scaling rather than merely speeding animations into flashes. Do not assume transparency preferences are universally supported: provide dependable opaque defaults/fallbacks and retain relevant accessible product settings.

## Web accessibility implementation targets

Target WCAG AA: 4.5:1 contrast for ordinary text, 3:1 for large text, and 3:1 for significant non-text control/focus visuals. Use WCAG's definition of large text rather than a community skill's simplified font threshold. Calculate actual colors; screenshots alone do not establish compliance.

Aim for at least 44×44 CSS px for primary touch targets as this skill's comfort target, not a claim about WCAG's minimum. Compact desktop controls can account for pointer precision and increase hit areas for coarse pointers. Accessible labels, visible focus, keyboard order, and screen-reader semantics matter equally. Use native button/a/input semantics. Custom controls require appropriate keyboard behavior, not just a role attribute.
