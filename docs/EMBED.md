# Embed Moonrise Special Prompt

Ways to point agents, docs, and sites at this repo.

## Raw prompt (best for agents)

```text
https://raw.githubusercontent.com/trymoonrise/moonrise-special-prompt/main/PROMPT.md
```

Ask the agent:

```text
Fetch the Moonrise Special Prompt from the raw URL above and apply it to this screen.
Keep every feature and all content. Use the unslop-style audit → direction → passes workflow,
and treat https://github.com/heydamir/unslop as the professional UI craft reference.
```

## GitHub blob (best for humans)

```text
https://github.com/trymoonrise/moonrise-special-prompt/blob/main/PROMPT.md
```

## Designer Tips live demos

```text
https://trymoonrise.com/designer-tips.html#craft
```

## HTML iframe

```html
<iframe
  title="Moonrise Special Prompt demos"
  src="https://trymoonrise.com/designer-tips.html#craft"
  loading="lazy"
  referrerpolicy="no-referrer-when-downgrade"
  style="width:100%;min-height:720px;border:1px solid #e5e5e5;border-radius:12px;background:#fff;"
></iframe>
```

## Markdown badges

```md
[![Designer Tips](https://img.shields.io/badge/Live_demos-Designer_Tips-111111?style=for-the-badge)](https://trymoonrise.com/designer-tips.html)
[![Moonrise](https://img.shields.io/badge/Product-trymoonrise.com-0A7C66?style=for-the-badge)](https://trymoonrise.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-2F6FED?style=for-the-badge)](LICENSE)
```

## Cursor project rule

Save `PROMPT.md` as `.cursor/rules/moonrise-special-prompt.mdc` (or symlink it) so every Cursor agent chat in that project starts with the same bar.
