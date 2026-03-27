# magicthegathering — Magic: The Gathering typesetting for LaTeX

Version 1.1 — 2026-03-21

## Description

The `magicthegathering` package provides LaTeX commands for typesetting
*Magic: The Gathering* content:

1. **Mana symbols** — inline coloured mana icons (`\mana{R}`)
2. **Full mana costs** — space-separated symbol lists (`\manacost{1 U U}`)
3. **Colour shortcuts** — `\manaW` through `\manaC`
4. **Set symbols** — expansion-set icons (`\setsymbol{mh3}`)
5. **Card hyperlinks** — clickable Scryfall links (`\card{Lightning Bolt}`)
6. **Custom-text card links** — `\cardlink{name}{text}`
7. **Sideboard guides** — formatted IN/OUT tables (`matchup` environment)
8. **Deck-list import** — read a plain-text file (`\insertdeck{deck.txt}`)
9. **Match results** — tournament tables with auto W-L-D records

## Quick start

```latex
\documentclass{article}
\usepackage{magicthegathering}
\begin{document}
\card{Lightning Bolt} costs \manacost{R}.
\end{document}
```

Compile with `lualatex --shell-escape` (for live SVG) or
`pdflatex` (with pre-converted PDFs).

## Symbol artwork

Mana and set symbols were last updated in December 2025.
Sets released after that date may not yet be included.
Updated artwork will ship with future releases.

## Documentation

See `magicthegathering-doc.tex` / `magicthegathering-doc.pdf` for full documentation with
live examples.

## Requirements

- TeX Live 2020+ or MiKTeX 21+
- Inkscape (only for live SVG rendering)

## Licence

- Package code: LPPL 1.3c or later
- SVG artwork: SIL Open Font Licence 1.1 (Mana/Keyrune by Andrew Gioia)

## Trademark

Magic: The Gathering, the mana symbols, the tap symbol, the set symbols,
and all associated card names and game elements are trademarks and/or
copyrighted materials of Wizards of the Coast LLC and/or its affiliates.
All rights in such materials are reserved by Wizards of the Coast.
This package is an unofficial fan project and is not produced, endorsed,
supported, or affiliated with Wizards of the Coast.

SVG artwork is from the Mana and Keyrune projects by Andrew Gioia,
released under the SIL Open Font Licence 1.1.

## Author

Hypergeomancer
