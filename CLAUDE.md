# CLAUDE.md

This is an awesome list repository — a curated list of IRC resources.

## Structure

- `readme.md` — The main awesome list content
- `contributing.md` — Contribution guidelines
- `readme-icons.md` — Legacy version of the list with inline icons (not actively used)

## List Entry Format

```md
- [Name](https://example.com) - Short description. ([source](https://github.com/example/repo)) `Tag`
```

Tags are either language (`Python`, `Go`, `Rust`, `C`, etc.) or platform (`Web`, `macOS`, `Windows`, `Linux`, etc.).

## Linting

The CI runs `awesome-lint` on `readme.md` and link checking via `lychee`. Run locally with:

```sh
npx awesome-lint readme.md
```

## Key Rules

- Only add actively maintained projects
- Each entry needs: name, link, short description
- Source code link is optional but preferred
- Keep descriptions concise (one sentence)
- Entries within sections are ordered by relevance/popularity
