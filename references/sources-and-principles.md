# Sources and design judgment

Reviewed: 2026-11-16. This document summarizes sources and provides original web adaptations. It does not reproduce the source project or equate community guidance with official rules.

## Sources

1. User-specified Apple design principles: https://developer.apple.com/cn/design/human-interface-guidelines/design-principles
   Official structured content: https://developer.apple.com/tutorials/data/cn/design/human-interface-guidelines/design-principles.json
   Static retrieval of the Chinese page requires JavaScript. During creation, the official English structured body was read and the Chinese structured endpoint was confirmed. English page: https://developer.apple.com/design/human-interface-guidelines/design-principles
2. dickwu/apple-design-skill: https://github.com/dickwu/apple-design-skill/blob/main/SKILL.md
   This skill borrows the review method of establishing context, consulting relevant references, distinguishing evidence from judgment, and proposing actionable improvements. It shifts the emphasis to content-led web generation, does not copy that project's reference collection, and does not require installing it.

## Concise interpretation of Apple's principles

Apple frames purpose, agency, responsibility, familiarity, flexibility, simplicity, craft, and delight as decision-making tools, not a single visual template. Help real people accomplish goals, retain control and recovery options, protect their data, establish consistent behavior, adapt to varied contexts, and improve the experience through details and appropriate emotion. Delight is not decoration; simplicity does not mean removing necessary functions.

## Original web adaptation

| Dimension | Design question | Observable delivery evidence |
|---|---|---|
| Purpose | What does the person most want to accomplish now? | Discoverable primary task and action; secondary content does not dominate |
| Agency | Can they go back, change, or cancel? | Preserved input, cancellation paths, undo where feasible |
| Responsibility | Are data use and consequences transparent? | Purposeful permissions, no default exposure of sensitive values, honest demo boundaries |
| Familiarity | Do labels and behaviors follow web expectations? | Links navigate, buttons act, browser Back works |
| Flexibility | Can work continue with another screen or input method? | Desktop/mobile core paths, keyboard operation, text scaling |
| Simplicity | Does organization make the task easier? | Clear grouping, progressive disclosure, explicit labels |
| Craft | Does the interface survive realistic boundaries? | Long titles, empty states, scrolling, and error recovery remain usable |
| Delight | Which detail expresses character without obstructing work? | Purposeful motion, feedback, or presentation, with reduced-motion support |

These mappings are this skill's implementation advice, not Apple quotations. Do not mechanically copy community prescriptions for native type sizes, touch sizes, appearance switches, or menus. Web uses CSS pixels and browser semantics. Consult the relevant official page when native platform rules matter.
