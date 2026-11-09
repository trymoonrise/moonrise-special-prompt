<p align="center">
  <a href="https://trymoonrise.com">
    <img src="https://trymoonrise.com/assets/MoonriseLogo.png" alt="Moonrise" width="72" height="72" />
  </a>
</p>

<h1 align="center">Moonrise Special Prompt</h1>

<p align="center">
  The official paste-anywhere UI prompt for <a href="https://trymoonrise.com">Moonrise Studio</a>.
  <br />
  Raise spacing, buttons, loading, focus, and empty states — without rebuilding the product.
</p>

<p align="center">
  <a href="https://trymoonrise.com/ui-library.html"><img src="https://img.shields.io/badge/Live_demos-Designer_Tips-111111?style=for-the-badge" alt="UI Library" /></a>
  <a href="https://trymoonrise.com"><img src="https://img.shields.io/badge/Product-trymoonrise.com-0A7C66?style=for-the-badge" alt="Moonrise" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-2F6FED?style=for-the-badge" alt="MIT" /></a>
  <a href="https://github.com/heydamir/unslop"><img src="https://img.shields.io/badge/UI_craft-unslop-111111?style=for-the-badge" alt="unslop" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/trymoonrise/moonrise-special-prompt?style=flat-square" alt="Stars" />
  <img src="https://img.shields.io/github/forks/trymoonrise/moonrise-special-prompt?style=flat-square" alt="Forks" />
  <img src="https://img.shields.io/github/last-commit/trymoonrise/moonrise-special-prompt?style=flat-square" alt="Last commit" />
  <img src="https://img.shields.io/github/license/trymoonrise/moonrise-special-prompt?style=flat-square" alt="License badge" />
  <img src="https://img.shields.io/badge/agents-Cursor%20%7C%20Claude%20%7C%20Codex%20%7C%20Copilot-111111?style=flat-square" alt="Agents" />
</p>

---

## Why this exists

Moonrise builds calm, modern local-business websites. Agents often invent purple gradients, broken loaders, missing contact facts, or flashy motion. This repo is the public **special prompt**: paste it into an agent that already has a project open.

Professional UI craft here is adapted from **[unslop](https://github.com/heydamir/unslop)** by Damir Sokolovsky (CC BY 4.0): audit the slop, set a direction from the product, then polish pass by pass so the screen stops looking AI-generated. See [`CREDITS.md`](CREDITS.md).

| You want | This repo gives you |
| --- | --- |
| Restyle the project you have open | [`PROMPT.md`](PROMPT.md) — paste the whole file into your agent |
| Every UI Library type as raw code | [`ui/`](ui/) — one folder per category, one HTML file per type |
| Live examples | [UI Library](https://trymoonrise.com/ui-library.html) on trymoonrise.com |
| Anti-slop craft reference | [heydamir/unslop](https://github.com/heydamir/unslop) |
| Generated site quality | Ship bar rules so incomplete or broken pages do not ship |

> Formerly published as `trymoonrise/craft`. Same project; clearer name.

---

## Quick start (2 minutes)

1. Open **[`PROMPT.md`](https://github.com/trymoonrise/moonrise-special-prompt/blob/main/PROMPT.md)**.
2. Copy the entire file (`raw` → select all → copy).
3. Paste it into Cursor, Claude, Codex, Copilot, or a similar coding agent that already has your project open.
4. Point at one screen or a few files: *“Apply the Moonrise Special Prompt to this page. Keep every feature and all copy.”*

The agent should keep routes, data, and behavior, then fix spacing, type, color, buttons, loading, hover/press, focus, and empty/error states.

### One-liner for agents

```text
Read https://raw.githubusercontent.com/trymoonrise/moonrise-special-prompt/main/PROMPT.md
and apply it to the current screen. Keep every feature and all content.
Download every file in ui/index.json before you invent a control.
```

### Embed the raw prompt

Use the raw URL anywhere an agent or script can fetch text:

```text
https://raw.githubusercontent.com/trymoonrise/moonrise-special-prompt/main/PROMPT.md
```

Markdown embed (GitHub will render a link preview in many clients):

```md
[Moonrise Special Prompt](https://github.com/trymoonrise/moonrise-special-prompt/blob/main/PROMPT.md)
```

HTML embed for docs sites:

```html
<iframe
  title="Moonrise Special Prompt"
  src="https://trymoonrise.com/ui-library.html#craft"
  loading="lazy"
  style="width:100%;min-height:640px;border:1px solid #ddd;border-radius:12px;"
></iframe>
```

---

## Repository map

```text
moonrise-special-prompt/
├── PROMPT.md                 # The special prompt (copy this)
├── before-after.html         # Playback: timeline, play, pause, ±15s
├── README.md                 # You are here
├── LICENSE                   # MIT
├── ui/                       # Every UI Library category and type, as raw code
│   ├── index.json            # The list an agent downloads in full
│   ├── css/                  # Shared styles and tokens
│   ├── sections/             # One folder per section category
│   ├── components/           # One folder per component category
│   └── screens/              # One folder per screen category
```

---

## Instructions by tool

### Cursor

1. Open your project.
2. Start Agent / Chat.
3. Paste `PROMPT.md`, or ask the agent to fetch the raw URL above.
4. Attach the files or `@folder` for the screen you want improved.
5. Optional: save `PROMPT.md` as a project rule (`.cursor/rules/moonrise-special-prompt.mdc`) so every chat starts with it.

### Claude / Claude Code

Paste the prompt at the top of the conversation, then name the files. For Claude Code, drop `PROMPT.md` into the project and say “follow Moonrise Special Prompt.”

### Codex / Copilot / other agents

Same pattern: full prompt first, then a short task. Do not ask the agent to invent a new design system if a preset already covers the control.

---

## UI library (raw code)

Every category and type from the [UI Library](https://trymoonrise.com/ui-library) is in [`ui/`](ui/). A category is a folder. A type is one HTML file: the markup, its class names, and a short properties note. Shared CSS is [`ui/css/ui-library.css`](ui/css/ui-library.css) and [`ui/css/ui-library-lab.css`](ui/css/ui-library-lab.css).

The prompt tells the agent to download **every** file listed in [`ui/index.json`](ui/index.json) into `.moonrise-ui/` before it designs. That gives it a base for how each control is built. It then uses the closest type, keeps the structure and states, and changes colors and labels only.

```text
https://raw.githubusercontent.com/trymoonrise/moonrise-special-prompt/main/ui/index.json
```

## Before and after

[`before-after.html`](before-after.html) is the playback an agent leaves with the work. Copy it into the project, keep the original files as **Before**, and record each pass through to **After**. The page is a simple HTML video: drag the timeline, press play or pause, or jump back and forward 15 seconds.

Live demos of the same types: **[UI Library](https://trymoonrise.com/ui-library.html)**

<p>
  <a href="https://trymoonrise.com/ui-library.html">
    <img src="https://trymoonrise.com/assets/MoonriseLogo.png" alt="Open UI Library on Moonrise" width="48" />
  </a>
</p>

---

## Design rules (summary)

The full rules live in [`PROMPT.md`](PROMPT.md), aligned with [unslop](https://github.com/heydamir/unslop). Short version:

- **Workflow** — audit → product direction → passes (spacing, color, icons, copy, type, layout, details, visuals, motion).
- **Spacing** on a 4px grid. No odd 7px / 13px values.
- **Color** — quiet chrome, one neutral ramp, one accent. No purple gradients, glows, glass blobs, or rainbow decoration.
- **Type / copy** — few sizes, two weights, sentence case, no hype or emoji chrome.
- **Buttons** — hover, press, disabled, stable loading (`aria-busy`).
- **Motion** — ~150–220ms, always with `prefers-reduced-motion`.
- **Forms** — visible focus rings, plain-language errors.
- **Layout** — mobile first, one composition, real product/place visuals, reserved image space.

### Finish bar

The prompt is done only when the open project still does what it did, and the screen looks finished: quiet color, consistent spacing, one button style, and real empty, error, hover, and focus states.

---

## How Moonrise uses this

| Surface | Role |
| --- | --- |
| [UI Library](https://trymoonrise.com/ui-library.html#craft) | Public copy button + live demos |
| Moonrise Studio | Designs each business site from its own facts |
| This GitHub repo | Source of truth for the public prompt and the `ui/` raw code |

Product: **[trymoonrise.com](https://trymoonrise.com)**  
Studio docs and demos: **[UI Library](https://trymoonrise.com/ui-library.html)**  
Main product source: **[trymoonrise/moonrise](https://github.com/trymoonrise/moonrise)**

---

## What this is not

- Not an npm package. `ui/` is raw reference code for agents, not a runtime install.
- Not a theme that restyles your whole app automatically.
- Not permission to invent features, change checkout, or rewrite auth.
- Not a substitute for your product’s real content and business facts.

---

## Contributing

1. Keep `PROMPT.md` the single source of the special prompt.
2. `ui/` is exported from the Moonrise UI Library. Change a pattern there, then re-export. Do not hand-edit the generated HTML.
3. Match the calm Moonrise visual language (near-black ink, soft fills, hairline borders).
4. Open a pull request with a short “why” — one concern per PR when possible.

Issues and PRs are welcome for clearer wording and agent-tool instructions.

---

## License

[MIT](LICENSE) © 2026 Moonrise

UI craft adapted from [unslop](https://github.com/heydamir/unslop) by Damir Sokolovsky, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Full attribution in [`CREDITS.md`](CREDITS.md).

---

<p align="center">
  <a href="https://trymoonrise.com">trymoonrise.com</a>
  ·
  <a href="https://trymoonrise.com/ui-library.html">UI Library</a>
  ·
  <a href="https://github.com/trymoonrise/moonrise-special-prompt/blob/main/PROMPT.md">PROMPT.md</a>
  ·
  <a href="https://github.com/heydamir/unslop">unslop</a>
</p>
