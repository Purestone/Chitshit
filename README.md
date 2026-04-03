# LaTeX Cheatsheet Template

A compact A4-landscape reference sheet layout — 7 columns, 5pt font, colour-coded markup. Compile with **XeLaTeX**.

---

## Setup

- Copy the file, keep the preamble unchanged, edit only the body
- Margins are extremely tight by design (max printable area)
- Font: Verdana via `fontspec` — swap for `DejaVu Sans` or `Arial` on Linux

---

## Custom Commands

| Command | Colour | Use for |
|---|---|---|
| `\hlhighlight{}` | Yellow bg | Major section banner |
| `\sectitle{}` | Dark blue | Sub-section heading |
| `\concept{}` | Teal | Key terms / vocabulary |
| `\procname{}` | Purple | Process names / steps |
| `\category{}` | Green bold | Category labels (Pros/Cons) |
| `\lbl{}` | Green bold | Inline key–value keys |
| `\lblnb{}` | Green plain | Softer inline labels |

---

## Usage Pattern
```latex
\hlhighlight{My Topic}
\sectitle{Sub-section}
\begin{itemize}
  \item \concept{Term:} definition.
  \item \category{Pros:} advantage.
\end{itemize}
```

---

## Fitting Content

- Shrink font: `\fontsize{4.5pt}{4.5pt}`
- More columns: change `\begin{multicols}{7}` to `{8}` or `{9}`
- Tighter gap: `\setlength{\columnsep}{5pt}`
- Force column break: `\columnbreak`

---

## Notes

- **Do not** use pdfLaTeX — `fontspec` requires XeLaTeX
- Works in Overleaf (set compiler to XeLaTeX)

---

## Licence

This repository is released under the [MIT Licence](https://opensource.org/licenses/MIT)
