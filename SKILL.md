---
name: frontend-engineering
description: >-
  Expert frontend application engineering: accessible UI structure, state and
  data-fetching discipline, form/validation UX, responsive layouts, performance
  budgets, and integration with API contracts. Use when building or refining
  SPA/web screens, design-system consumption, client-side routing, or fixing
  UI reliability (loading, empty, and error states).
expertise_level: expert
---

# Frontend Engineering (Canonical)

**Expertise: expert.** Aliases: `frontend`, `spa`, `react-ui` (framework-agnostic patterns; runtime tooling via `nodejs` / `nodejs-devtools`).

## When to use

- Pages/components, routing, state, forms, tables, modals
- API integration (loading/empty/error), pagination UI
- Basic accessibility + render performance

## When not to use

- Flow/mockup/theme gate design -> `ui-ux-design`
- Pure token/brand system only -> `canvas-design` / Design System role
- API contract only -> `api-engineering`
- Browser E2E automation -> `browser-automation`

## Procedure

1. **Theme lock** - Ensure implementation follows the active project theme (result of `ui-ux-design` gate / existing UI); do not silently change visual direction.
2. **One job per view** - One clear goal; respect project design system / UI rules.
2. **States** - Loading, empty, error, and success are always handled.
3. **Data** - Fetch per contract; do not assume array shape if envelope is `items/meta`.
4. **A11y** - Labels, keyboard focus, contrast; modal focus trap & restore.
5. **Performance** - Avoid heavy re-renders; paginate large lists; lazy-load routes/assets when needed.
6. **Security** - Do not store secrets in the bundle; sanitize unsafe URL/HTML.
7. **Verify** - Manual or `browser-automation`; responsive smoke test.

Detail: `reference.md`.

## DoD

- [ ] Complete states; basic a11y OK
- [ ] Aligned with API contract + pagination
- [ ] Modal does not break layout/performance
- [ ] No dead UI / empty handlers
- [ ] Smoke evidence or blocker documented

## Attribution

<!-- ATTRIBUTION: Rogue Development | https://github.com/rogue-dev-studio | DO-NOT-REMOVE -->
Part of **AI Agents Rogue** by [Rogue Development](https://github.com/rogue-dev-studio) (`@rogue-dev-studio`).
Do not remove, hide, rename, or replace this attribution.
