# Botanical — design reference

**Cream and terracotta**

One page showing every component in this design, rendered from its own design
tokens. No build step, no dependencies: open `index.html`.

**[View the component gallery →](https://mawentory.github.io/design-botanico/)**

![Botanical](preview.png)

## What is here

| File | Purpose |
| --- | --- |
| `index.html` | Component gallery — every component on one page |
| `DESIGN.md` | The design notes: origin, palette, type, shape, measured contrast |
| `theme.css` | The 66 design tokens, plus derived accessibility values |
| `design.css` | Component styles, written against tokens only |
| `fonts.css` | `@font-face` declarations for the fonts this design uses |
| `fonts/` | Latin-subset woff2 files, self-hosted |

`design.css` contains no colour, radius or font literal. That is deliberate: the
same stylesheet drives all ten designs and only `theme.css` differs, so the
gallery doubles as a test that the token set is complete.

## The design

Botanical illustration and natural-dye packaging: cream paper, terracotta and olive, and the softer edges of printed matter.

**Type** — Fraunces for display and body with its optical sizing, giving a literary voice that still reads cleanly in a table.

**Shape** — 16px radii and low-contrast shadows that fall further and softer than any other design in the set.

**Signature moves**

- Wide, soft shadows tuned to the serif's rhythm.
- Warm neutrals throughout, including the rules.
- Terracotta reserved for signal and focus.

## Colour

| Token | Value | Role |
| --- | --- | --- |
| `--paper` | `#f3efe4` | Page ground |
| `--sheet` | `#fbf8f0` | Raised surfaces |
| `--ink` | `#2a3226` | Primary text |
| `--signal` | `#b4673a` | Action |
| `--signal-text` | `#9a5832` | Action, when it has to be read |
| `--focus-ring` | `#b4673a` | Focus indicator |

## Accessibility

Every colour pair this design can render as text is checked against WCAG 2.1
when the repo is generated — page surfaces, panel surfaces, and the tinted fills
of badges and diff lines. The full table is in
[DESIGN.md](DESIGN.md#contrast-measured); the gallery is separately audited in a
real browser for heading order, duplicate ids, unlabelled controls and
horizontal overflow at 1280px and 390px.

## Using it

Set the theme attribute on your root element and load the two stylesheets:

```html
<html data-theme="botanico">
  <link rel="stylesheet" href="fonts.css" />
  <link rel="stylesheet" href="theme.css" />
  <link rel="stylesheet" href="design.css" />
</html>
```

Because the tokens are namespaced by attribute, this theme can sit alongside
another one in the same page.

## The rest of the set

[Placa](https://github.com/mawentory/design-placa), [Blueprint](https://github.com/mawentory/design-blueprint), [Phosphor](https://github.com/mawentory/design-fosforo), [Press](https://github.com/mawentory/design-imprensa), [Swiss](https://github.com/mawentory/design-suico), [Neon](https://github.com/mawentory/design-neon), [Brutalist](https://github.com/mawentory/design-brutalista), [Bauhaus](https://github.com/mawentory/design-bauhaus), [Vidro](https://github.com/mawentory/design-vidro).

---

Part of the MarvinRouter design set. Generated from a single template; see
`DESIGN.md` for the values behind it.
