# RTL, Accessibility, and Responsive Design

## Arabic and bidirectional layouts
- Set `dir="rtl"` at the correct document or application boundary for Arabic experiences.
- Use logical CSS properties such as `margin-inline-start`, `padding-inline-end`, and `border-inline-start` instead of assuming left/right.
- Ensure navigation, breadcrumbs, drawers, and directional icons behave correctly in RTL.
- Keep mixed Arabic/Latin strings, email addresses, codes, and identifiers readable; use direction isolation where necessary.
- Test Arabic fonts and line wrapping with realistic labels.
- Do not mirror universal symbols such as play, search, or some brand marks without reason.
- Check currency, decimal separators, dates, phone numbers, and table column order against the target locale.

## Accessibility
- Use semantic HTML and a logical heading structure.
- Associate every form control with a visible label.
- Ensure keyboard access and visible focus indicators.
- Provide accessible names for icon-only controls.
- Do not use color as the only status signal.
- Respect `prefers-reduced-motion`.
- Maintain sufficient contrast for text, controls, focus rings, and meaningful graphics.
- Make errors specific and programmatically associated with the relevant fields where feasible.
- Keep touch targets practical for mobile usage.

## Responsive strategy
Design for content and workflow rather than specific device mockups alone.
- Wide desktop: use available space for useful context and multi-column workflows.
- Tablet: collapse low-priority panels and adjust navigation.
- Mobile: prioritize the core task, reduce secondary columns, and provide explicit alternatives to dense desktop tables.
- Prevent horizontal overflow except where a deliberately scrollable data region is appropriate.
- Test long labels, translated text, zoom, and narrow viewports.

## Motion
- Use motion to show cause and effect, hierarchy, or state changes.
- Keep transitions brief and non-blocking.
- Avoid motion that delays common tasks.
- Honor reduced-motion preferences.
