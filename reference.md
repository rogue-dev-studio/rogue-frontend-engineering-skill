# Frontend Engineering - Reference

## State model

- Server state vs UI state separated clearly
- Derive state instead of duplicating it
- Optimistic UI only with a rollback path

## Forms & tables

- Associated labels; inline errors; disable submit while busy
- Tables: No. column when the list is paginated; clear page controls
- No decorative cards without interaction (see rule `ui`)

## Modal / overlay

- Portal/stacking context; scroll lock; focus restore
- Do not shift layout behind; close on Escape when the project pattern allows

## Performance

- Avoid lists without virtualization/pagination
- Image/media: appropriate size & lazy loading
- Bundle: code-split heavy routes

## Anti-patterns

- Fetch inside a tight loop without cache
- Ignore error boundary / silent failure
- Inline style chaos that fights design tokens
