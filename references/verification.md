# Delivery verification

## Representative scenarios

Choose real product tasks; do not add a test framework for a small screen:
- Success: find the primary action, complete the task, and confirm feedback matches data.
- Direct failure/recovery: network failure, invalid input, or no results; preserve input and context.
- Keyboard: Tab order, visible focus, Enter/Space, dialog Escape behavior, and focus restoration.
- Mobile: navigation, form fields, and primary actions remain reachable on narrow screens and with the virtual keyboard.

## Visual and responsive checks

Suggested samples: 1440px desktop, 1024px compact window, 390px phone, and 320px narrow screen. These are test samples, not mandated breakpoints. Check both sides of important content breakpoints and landscape where available. Do not rely solely on full-page screenshots.

Inspect actual rendering at the page top/bottom, sticky bars during scrolling, dialogs, longest titles, long Chinese copy, large numbers, empty lists, and error states. Look for unintended horizontal overflow, occlusion, broken wrapping, cramped targets, or falsely interactive elements. Deliberate table scrolling should be discoverable without widening the entire page.

Test 200% text/page zoom, implemented light/dark themes, reduced-motion, keyboard focus, and touch. Screenshots cannot prove screen-reader usability or passing contrast; use actual values or interaction evidence.

## Engineering checks

Inspect package scripts first; lint with --fix is not a read-only check. Run the nearest existing type/build/test checks and preserve the user's working tree. Disclose missing tests or environment blocks. Do not add test frameworks or dependencies merely to complete this checklist.

When a browser/runtime is available: capture, inspect, fix, and recheck. Otherwise deliver code and run instructions, explicitly stating that browser visual verification has not been performed. Do not claim cross-browser or physical-device verification without doing it. Chrome responsive mode is not an iOS Safari device test.

## Completion criteria

The primary task works, supported viewport samples have no blocking issues, relevant states and accessibility paths have been checked, and build status is clear. Stop unrelated polishing. Report locations, two or three design reasons, actual tests, and limitations. Do not claim Apple certification, 100% HIG compliance, or guaranteed review acceptance.
