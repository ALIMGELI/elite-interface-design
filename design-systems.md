# Design Systems

## Token architecture
Define tokens by semantic role, then map them to theme values. Example names:
- `--color-canvas`
- `--color-surface`
- `--color-surface-raised`
- `--color-text`
- `--color-text-muted`
- `--color-border`
- `--color-primary`
- `--color-primary-hover`
- `--color-success`
- `--color-warning`
- `--color-danger`
- `--space-1` through `--space-8`
- `--radius-sm`, `--radius-md`, `--radius-lg`
- `--shadow-sm`, `--shadow-md`
- `--font-body`, `--font-display`
- `--text-xs` through `--text-2xl`

These names are illustrative; adapt to the codebase rather than introducing needless churn.

## Component contracts
For each reusable component, define:
- Purpose and when to use it.
- Variants and sizes.
- Required and optional properties.
- Default, hover, focus, pressed, disabled, loading, selected, and error states where relevant.
- Keyboard behavior and accessible name/label.
- Responsive behavior.

## Core component set
Select what the product needs:
- Button, icon button, link.
- Text input, search, select, checkbox, radio, switch.
- Tabs, breadcrumb, pagination.
- Table, data row, filter bar, toolbar.
- Dialog, drawer, tooltip, toast/alert.
- Card, metric, chart container.
- Badge/status label.
- Empty state, skeleton/loading, error state.
- Navigation rail/sidebar, top bar, mobile navigation.

## Consistency
- Prefer one clear primary button style and a small number of variants.
- Reuse spacing and type tokens.
- Keep icon size, stroke style, and alignment consistent.
- Avoid one-off colors unless they encode a meaningful status or brand accent.
- Document exceptions rather than allowing silent inconsistency.

## Theme support
If light/dark themes are requested, map semantic tokens for each theme. Do not invert colors mechanically; check contrast, shadows, borders, charts, overlays, and focus states in both themes.
