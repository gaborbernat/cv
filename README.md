[![View PDF](https://img.shields.io/badge/View%20as%20PDF-latest%20CV-blue?style=flat-square&logo=docusign)](https://gaborbernat.github.io/cv/main.pdf)
![Build LaTeX document](https://github.com/gaborbernat/cv/workflows/Build%20LaTeX%20document/badge.svg)

Contains my resume as a LaTeX document.

## Building

Requires [TeX Live](https://www.tug.org/texlive/) with packages `sectsty`, `dashrule`, and `ifmtarg`.

On macOS via Homebrew:

```bash
brew install texlive
```

Build the PDF:

```bash
pdflatex main.tex
```

## Pre-commit

Uses [pre-commit](https://pre-commit.com/) for formatting (LaTeX via [tex-fmt](https://github.com/WGUNDERWOOD/tex-fmt),
Markdown via [mdformat](https://github.com/hukkin/mdformat), YAML via [yamlfmt](https://github.com/google/yamlfmt)):

```bash
pre-commit install
pre-commit run --all-files
```
