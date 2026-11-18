# Domain docs

This repo uses a **single-context** domain documentation layout.

## Layout

- **Root glossary**: `GLOSSARY.md` (create when needed). One canonical place for project terminology.
- **Architecture Decision Records (ADRs)**: `docs/adr/` (one markdown file per decision).
- **Domain maps**: not required for single-context. If the repo grows into multiple bounded contexts, migrate to a root `GLOSSARY-MAP.md` that points to per-context `GLOSSARY.md` files.

## Consumer rules (for agents/skills)

- Before proposing or editing code that introduces or changes domain terms, consult `GLOSSARY.md` if present.
- Prefer adding/adjusting ADRs under `docs/adr/` for significant architectural decisions rather than burying rationale in issue comments only.
- Keep terminology consistent with existing docs; when in doubt, ask or record the term in `GLOSSARY.md`.

## Notes

- Monorepo/multi-context signals were not detected at setup time; revisit this file if that changes.
