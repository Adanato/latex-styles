# latex-styles

Shared LaTeX style files for research project logs and papers.

## Styles

| File | Description |
|------|-------------|
| `meeting.sty` | Meeting/dev log formatting: agenda items, action items, decision boxes |
| `section.sty` | Custom section and subsection heading styles |
| `colored_box.sty` | Colored tcolorbox environments for motivation, findings, and notes |
| `utils.sty` | Utility macros (`\todo`, etc.) |

## Usage

Add as a git submodule at `styles/` in your LaTeX project:

```bash
git submodule add git@github.com:Adanato/latex-styles.git styles
```

Then in your `.tex` file:

```latex
\usepackage{styles/meeting}
\usepackage{styles/section}
\usepackage{styles/colored_box}
\usepackage{styles/utils}
```

## Updating

To pull the latest styles into a consumer repo:

```bash
git submodule update --remote styles
git add styles
git commit -m "Update latex-styles submodule"
```
