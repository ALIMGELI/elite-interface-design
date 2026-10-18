# Enterprise and Business Interfaces

## Operating principle
Business software should feel polished while helping users complete frequent tasks quickly, accurately, and with confidence.

## Application shell
- Use stable navigation, a clear page title, breadcrumbs when helpful, and contextual actions.
- Distinguish global navigation from page-level tabs and filters.
- Keep active navigation states unmistakable.
- Provide account, branch, company, or workspace context where the product requires it.

## Dashboards
- Prioritize metrics that drive decisions, not decorative numbers.
- State units, date ranges, comparison periods, and metric definitions when relevant.
- Use charts only when they reveal patterns better than a table or summary.
- Pair colors with labels/icons; do not encode status by color alone.
- Avoid charts with fabricated claims; sample data should be identified as demo data.

## Tables
- Align text and numbers consistently; use tabular numerals for amounts.
- Provide useful column names, sensible widths, row hover/focus, and clear selected states.
- Add search, filters, sorting, pagination, and bulk actions only where they solve real tasks.
- Handle long values, empty results, loading, errors, and large datasets.
- On small screens, use a deliberate alternative: horizontal scroll, prioritized columns, or a record-detail view.

## Forms
- Group fields by workflow, not arbitrarily.
- Mark required fields clearly and use correct input types.
- Provide inline validation and explain how to correct errors.
- Keep labels visible; do not rely on placeholders as labels.
- Use progressive disclosure for advanced fields when it reduces cognitive load.
- Confirm save, submit, approve, post, or delete outcomes.

## Financial screens
- Clearly label currency and units; avoid ambiguous amounts.
- Use consistent decimal precision and right/left alignment appropriate to locale.
- Separate subtotal, tax, discount, paid, due, and total values.
- Distinguish draft, pending, approved, posted, reversed, and cancelled states when applicable.
- Never represent demo calculations as audited accounting logic.
- Destructive or irreversible financial actions require clear confirmation and an audit-friendly interaction pattern.

## POS and inventory
- Optimize item lookup, scanning, quantity changes, discounts, customer selection, payment, and receipt workflows.
- Keep the current transaction summary visible when useful.
- Show stock units, availability, and warnings without excessive noise.
- Support keyboard/touch targets appropriate to the environment.
- Make stock and payment states explicit.

## HR and project management
- Use clear statuses, owners, dates, filters, and permission-aware actions.
- Handle confidential data carefully in examples and avoid real personal data.
- Distinguish planned, active, blocked, completed, and cancelled work.
- Provide audit trails or change history when the workflow needs accountability.

## Enterprise design anti-patterns
- Too many summary cards.
- Tiny low-contrast table text.
- Overuse of pill badges.
- Hidden primary actions.
- Every action styled as primary.
- Filters that reset unexpectedly.
- Modals for workflows that need full pages.
- Fake controls and fake backend claims.
