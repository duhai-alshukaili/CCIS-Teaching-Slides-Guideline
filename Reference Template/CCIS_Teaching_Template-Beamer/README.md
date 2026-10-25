# CCIS Beamer theme

Beamer version of the CCIS course slide template, built to the *CCIS Guideline for Teaching Slide Decks*.

## Files

| File | Purpose |
|---|---|
| `beamerthemeCCIS.sty` | The theme. Keep it next to your `.tex` file, or upload it to the Overleaf project. |
| `utas-logo.png` | Official UTAS logo (staff PNG). Do not replace, redraw or recolor it. |
| `lecture-template.tex` | Sample lecture following the guideline's skeleton (Section 10). Copy it for each lecture. |
| `references.bib` | Bibliography for the APA 7 reference list. |
| `lecture-template.pdf` | The compiled sample. |

## Build

```
latexmk -pdf lecture-template.tex
```

You can also use XeLaTeX or LuaLaTeX. Bibliographies need biber (Overleaf runs it automatically). Compile twice so the section dividers and the agenda can list every part. Fonts are Atkinson Hyperlegible for text and Source Code Pro for code, from the `atkinson` and `sourcecodepro` packages in TeX Live. If either package is missing, the theme falls back to Helvetica and Inconsolata.

## Set once per course, then per lecture

```latex
\documentclass[aspectratio=169,10pt]{beamer}
\usetheme{CCIS}
\coursecode{COMP3105}  \coursetitle{Information Retrieval}
\branch{Ibri}          \semester{Fall 2026/2027}
\lecturenumber{4}      \title{Vector space model}   \author{Dr. ...}
\acknowledgment{Acknowledgment: ...}
```

## What the theme gives you

| Command | Result |
|---|---|
| `\titleframe` | Title slide: college name, UTAS logo top right, course, lecture, lecturer and branch, semester, acknowledgment line |
| `\section{Name}` | A navy section divider: "Part n of N", the part names along the bottom with the current one marked. Put `\partquestion{...}` (bridging question) and `\partoutcome{...}` before it. Load the theme with `[nodividers]` to turn this off. |
| `\agendalist` | Agenda built from the sections |
| `\framesubtitle{...}` | Small label above the headline. If you leave it out, the label is "Part n · section" |
| `\source{...}` | Source line at the bottom of the frame, at the 14 pt equivalent |
| `\clo{2}`, `\lastlecture{...}` | Outcome tags and the link to the previous lecture |
| `\options{A}{B}{C}{D}`, `\checklabel`, `\nextlink{...}` | Check-for-understanding frame |
| `nextsteps` environment with `\nextstep{Lab}{...}` | Next-steps panel |
| `\evidencebox` | Placeholder box for evidence still to come |
| `\cornerlogo` | Small UTAS logo, top right (closing frames) |
| `lstlisting` | Code style: Source Code Pro at the 19 pt equivalent. Wrap the key line in `<@ ... @>` to highlight it. |
| pgfplots styles `ccis axis`, `ccis a`, `ccis b`, `ccis c` | Chart series that differ by line style and marker, not by color alone |

Sizes: a 16:9 Beamer frame is 160 mm wide, so multiply by about 2.1 to get the PowerPoint point size the guideline uses. The 16 pt headline = 34 pt, 10 pt body = 21 pt, 6.8 pt footer and source lines = 14 pt.

## Accessibility note

PDFs that pdfLaTeX produces are poorly tagged for screen readers (Guideline Section 6). Upload the PDF to the LMS, and provide an accessible version on request.
