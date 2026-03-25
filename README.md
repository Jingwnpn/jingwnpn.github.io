# jings.design — Portfolio

Personal portfolio for **Jing W. Pan**, Senior Product Designer.

Live at [jings.design](https://jings.design)

---

## Project

A single-page terminal-style portfolio. The aesthetic concept: a retro CLI interface with a dark/light theme, boot sequence, interactive terminal commands, and traditional web layout sections for case studies, experience, and about.

Built as a single self-contained HTML file — no framework, no build step, no dependencies beyond a Google Fonts import.

---

## Files

| File | Description |
|------|-------------|
| `index.html` | Main portfolio — all HTML, CSS, and JS in one file |
| `404.html` | Custom 404 page matching portfolio aesthetic |

---

## Design system

**Font:** JetBrains Mono (400 weight only)

**Themes:** Dark (default) and light, toggled via footer button. CSS variables throughout.

**Key CSS variables:**
- `--bg` / `--bg2` / `--bg3` — background layers
- `--fg` — primary text
- `--fg-dim` — secondary text (muted, passes WCAG AA)
- `--fg-mute` — decorative/disabled text
- `--accent` / `--hi` — primary highlight (same value)
- `--hi-dim` — secondary highlight
- `--ok` — green used for boot sequence check marks
- `--border` — dividers and borders
- `--danger` — error states

**Breakpoints:**
- `≤700px` — stacks layouts, switches experience table to card list, shrinks terminal header box, hides "press 0–3" footer hint
- `≤480px` — dropdown nav replaces top nav, hides case study name column

---

## Sections

| Nav | ID | Description |
|-----|----|-------------|
| 0. Home | `sec-home` | HELLO! ASCII, info card, interactive terminal |
| 1. Case Studies | `sec-projects` | Table + preview card. Detail pages: `sec-spacewalk`, `sec-obsidian`, `sec-playstation` |
| 2. Experience | `sec-experience` | Work history + education table (desktop) / card list (mobile) |
| 3. About | `sec-about` | Bio prose, skills tags, contact |

---

## Terminal

The home page contains a functional CLI terminal. Commands:

| Command | Description |
|---------|-------------|
| `whoami` | Background and philosophy |
| `ls` | List case studies |
| `open spacewalk` / `open obsidian` / `open playstation` | Navigate to case study detail page |
| `git log` | Career timeline as git commits |
| `cat contact` | Contact info |
| `help` or `?` | Show available commands |
| `clear` | Reset terminal to initial boot state |
| `0` `1` `2` `3` | Navigate sections by number |

The boot sequence on load shows: header box → credential rows → progress bar → available commands.

---

## Deploying changes

```bash
git add .
git commit -m "describe change"
git push
```

GitHub Pages redeploys automatically within ~1 minute.

---

## Owner

Jing W. Pan · [jingwnpn@gmail.com](mailto:jingwnpn@gmail.com) · [linkedin.com/in/jingwenpan](https://linkedin.com/in/jingwenpan)
