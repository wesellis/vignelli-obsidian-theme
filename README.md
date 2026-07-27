# Vignelli

A serif, rule-driven theme for [Obsidian](https://obsidian.md) — a screen port of the "Vignelli reference" print house style. **Chalkboard black · bone white · gold.**

Massimo Vignelli aesthetic: **serif type** (Bodoni display / Georgia body), a **rigorous grid**, and a strict **rule hierarchy carried in gold**. Headers, dividers (`---`), and table bars are gold in *both* themes; the black/bone ground simply reverses.

> *"The life of a designer is a life of fight: fight against the ugliness."* — Massimo Vignelli

---

## The palette

| | Background | Body text | Headers · dividers · table bars | Highlight |
| --- | --- | --- | --- | --- |
| **Dark** | black `#2F2F2F` | white `#F8F4F9` | gold `#D1AC23` | teal `#74D2B4` |
| **Light** | white `#F8F4F9` | black `#2F2F2F` | gold `#D1AC23` | teal `#74D2B4` |

Gold and teal are pinned across both modes; the black/white pair swaps. **Gold** carries structure (headers, rules, table bars, links, accents); **teal** is the highlighter and selection color. Nothing else is tinted — hierarchy is expressed through gold rule weight, not scattered color.

---

## What it does

- **Type** — Bodoni (Moda → Didot → Bodoni MT) for headings, Georgia for reading, Courier for code. A proper perfect-fourth type scale so H1 reads as a masthead, not a Word heading.
- **Headers on gold rules** — H1 on a gold masthead rule, H2 on a gold hairline; `---` is the gold divider.
- **Tables** — the header sits between gold bars, the body closes on a gold bar, hairline rules between rows. No vertical lines, no zebra, tabular numerals.
- **Callouts** — a faint panel with a gold left rule and a gold small-caps label (a Vignelli set-off, not a docs-site admonition box).
- **Code** — syntax **desaturated into the palette**: bone body, muted-italic comments, gold keywords — in reading, live-preview *and* source mode.
- **Everything else** — links, tags, checkboxes, properties, embeds, graph, canvas, math, mermaid, scrollbars, tooltips, and a print stylesheet, all in chalkboard/bone/gold.

---

## Multiple highlight colours

Native Obsidian gives you exactly **one** highlight color. Vignelli adds six tones — **teal, gold, rust, slate, plum, rose** — two ways:

**No plugin required** — combine `==highlight==` with an inner wrapper:

| Markup | Colour |
| --- | --- |
| `==text==` | teal `#74D2B4` (default) |
| `==**text**==` | gold |
| `==*text*==` | rust |
| `==~~text~~==` | slate |

These render identically in reading, live-preview, and source mode.

**With the [Highlightr](https://github.com/chetachiezikeuzor/Highlightr-Plugin) plugin** (for a color menu / all six + more): set Highlightr's method to **"CSS classes"**, and name your highlights `teal`, `gold`, `rust`, `slate`, `plum`, `rose` (common names like `mint`, `green`, `yellow`, `red`, `blue`, `purple`, `pink` are mapped too). The plugin then emits `<mark class="hltr-…">`, which this theme styles.

So: multi-color highlighting works out of the box, and the plugin is optional sugar.

---

## Install

1. Open your vault's `.obsidian/themes/` folder.
2. Create a `Vignelli` folder inside it and copy in `manifest.json` + `theme.css`:

```
<vault>/.obsidian/themes/Vignelli/
├── manifest.json
└── theme.css
```

3. **Settings → Appearance → Themes → Vignelli.**

---

## Style Settings

Install the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin for live controls (all optional; defaults are baked in):

| Setting | Default |
| --- | --- |
| Display / body / mono fonts | Bodoni · Georgia · Courier |
| Body size · line height · reading width | 18 px · 1.6 · 40 rem |
| **Gold** (themed color picker) | `#D1AC23` |
| **Highlight** teal (themed color picker) | `#74D2B4` |
| Gold headings | on |
| Uppercase H1 masthead | off |
| Justify body text | off |
| Hide inline title | off |

---

## Fonts

Fonts match the original Vignelli doc engine: headings use **Bodoni MT** (ships with Microsoft Office / Windows), body uses **Georgia**, code uses **Courier New**. If Bodoni MT isn't present, headings fall back through Bodoni 72 → Bodoni Moda → Didot → Georgia. Point the Style Settings font fields anywhere you like.

---

## Provenance

The visual language derives from `vignelli.py`, the house-style engine that typesets these documents for print — the same rule hierarchy and type pairing, retuned for a screen and dressed in chalkboard/bone/gold.

## License

MIT © Wesley Ellis
