# Contributing to Moonrise Special Prompt

Thanks for helping keep the Moonrise Special Prompt clear and useful.

## Scope

This repo holds:

- `PROMPT.md` — the paste-anywhere special prompt
- `presets/` — small HTML/CSS snippets agents can paste and recolor
- Docs that explain how to use them with coding agents

It does **not** hold the Moonrise Studio app. Product changes belong in [trymoonrise/moonrise](https://github.com/trymoonrise/moonrise).

## Guidelines

1. Prefer clearer wording over new sections.
2. Keep presets dependency-free and under a few KB.
3. Match UI Library patterns: calm surfaces, 4px spacing, one accent, real hover/press/focus/loading.
4. Keep the [unslop](https://github.com/heydamir/unslop) credit (CC BY 4.0) in `PROMPT.md` / `CREDITS.md` when adapting anti-slop craft rules.
5. Do not add purple gradients, glows, emoji chrome, or noisy infinite motion.
6. One concern per pull request when you can.

## Pull requests

- Title: short “why” (for example `Clarify ship bar for generated sites`).
- Describe what an agent should do differently after the change.
- Link a UI Library section if the change mirrors a live demo.

## Questions

Open an issue, or start from the live demos on [UI Library](https://trymoonrise.com/ui-library.html).
