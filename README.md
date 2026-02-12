# Hintium <picture><source media="(prefers-color-scheme: dark)" srcset="img/icon_header_dark.svg"><source media="(prefers-color-scheme: light)" srcset="img/icon_header.svg"><img alt="" src="img/icon_header.svg" width="40" height="56"></picture>

**Vimium-style keyboard hint navigation for all JetBrains IDEs.**

Press a shortcut and every actionable element in the IDE lights up with a letter hint. Type the letters to click it — no mouse needed. Works across the entire IDE, not just the editor.

---

## Features

- **Hint overlay on everything** — Buttons, tabs, tool windows, trees, lists, tables, editor tabs, navigation bar, terminal buttons, and more all get letter hints.
- **Home-row-first hints** — Hint characters start from `a s d f g h j k l` so your fingers barely move.
- **QMK-style combos** — Press two keys simultaneously to trigger any IDE action or synthesize a keypress. Combos are order-independent (`D+K` = `K+D`) and work even while hints are active.
- **Customizable appearance** — Adjust hint background color, matched-character color, text color, font size, and opacity to match your theme.

## Installation

Install directly from the JetBrains Marketplace:

1. Open **Settings** > **Plugins** > **Marketplace**
2. Search for **Hintium**
3. Click **Install** and restart the IDE

## Usage

### Hint navigation

1. Press **Ctrl+Alt+Shift+Space** to activate the overlay.
2. Letter hints appear on all actionable UI elements.
3. Type the hint letters to activate that element. Matched characters highlight as you type.
4. Press **Escape** or the activation shortcut again to dismiss.

### Combos

Combos let you trigger actions by pressing two keys at the same time (within a configurable time window). Enable them in **Settings** > **Tools** > **Hintium**.

Default combos (when enabled):

| Keys | Action |
|------|--------|
| `D` + `K` | Toggle hint overlay |
| `F` + `J` | Escape |

Each combo can either:
- **Execute an IDE action** — chosen from a searchable list of all registered actions.
- **Synthesize a keypress** — sends a keypress (with optional modifiers) to the OS.

## Configuration

All settings are under **Settings** > **Tools** > **Hintium**:

| Setting | Description |
|---------|-------------|
| Hint colors | Background, matched-character background, and text color (with opacity) |
| Hint font size | Size of the hint label text |
| Enable combos | Toggle the combo system on/off |
| Combo term | Time window (ms) for recognizing simultaneous key presses |
| Combo table | Add, edit, or remove combos — map key pairs to IDE actions or synthesized keypresses |

## Compatibility

Works with **all JetBrains IDEs** — IntelliJ IDEA, WebStorm, PyCharm, GoLand, CLion, Rider, RubyMine, DataGrip, Android Studio, and others.

**Requirements:** Java 17 &bull; IntelliJ Platform 2024.3+
