# Quality Checklist and Review Rubric

Use this checklist before delivery. Mark each item as Pass, Needs work, or Not applicable, and provide evidence for important claims.

## Product and UX — 20 points
- [ ] Main task and primary action are immediately clear.
- [ ] Navigation matches the user's mental model.
- [ ] Content hierarchy reflects task importance.
- [ ] Forms and tables support realistic workflows.
- [ ] Empty, loading, success, and error states are considered.

## Visual craft — 20 points
- [ ] Composition has a deliberate visual point of view.
- [ ] Typography, spacing, color, and surfaces are coherent.
- [ ] The interface is distinctive without sacrificing clarity.
- [ ] Density is appropriate to the product.
- [ ] No unnecessary decoration or generic repeated card grids.

## Design system — 15 points
- [ ] Tokens are used consistently.
- [ ] Component variants and states are coherent.
- [ ] Iconography and control sizing are consistent.
- [ ] Similar patterns behave similarly across screens.

## Implementation — 15 points
- [ ] Existing project conventions were respected.
- [ ] Code is readable and maintainable.
- [ ] Interactive controls perform their stated action.
- [ ] No dead buttons or misleading functionality.
- [ ] No unnecessary dependencies or console/build errors known to the tools used.

## Responsive behavior — 10 points
- [ ] Wide and narrow layouts are considered.
- [ ] Content does not overflow unintentionally.
- [ ] Dense tables have a mobile strategy.
- [ ] Touch and keyboard interactions remain usable.

## Accessibility and localization — 10 points
- [ ] Labels, semantics, focus, and contrast are considered.
- [ ] Status is not conveyed by color alone.
- [ ] RTL/LTR behavior is correct where applicable.
- [ ] Reduced motion is considered when animation is present.

## Verification and delivery — 10 points
- [ ] Main workflow was tested where tools permit.
- [ ] Claims match actual tests performed.
- [ ] Run/preview instructions are included.
- [ ] Limitations and unfinished areas are disclosed.

## Scoring guidance
Total: 100 points. Use scores to identify weaknesses, not to claim objective perfection. A score above 90 should require strong evidence across all applicable categories. If the environment cannot provide browser rendering or screenshots, explicitly state that visual verification remains incomplete.

## Final quick pass
1. Can a new user tell what to do first?
2. Is the design specific to this product?
3. Is the most frequent workflow fast?
4. Are all controls understandable and functional?
5. Does the layout still work with real-length content?
6. Are Arabic/RTL or other localization requirements verified?
7. What is the most important remaining defect?
