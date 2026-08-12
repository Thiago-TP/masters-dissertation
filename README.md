# Master Thesis — Project Files

This repository contains the LaTeX source, figures, tables and build artifacts for my master's dissertation and accompanying presentation.

> [!WARNING]
> For building the project, a full TeX distribution is required (TeX Live recommended) including packages for TikZ/PGF, pgfplots and common `bib` backends.


**Project Overview**
- **Purpose:** Source files and assets for the author's master's dissertation (LaTeX) and a Beamer presentation.
- **Main output:** A compiled PDF of the thesis (usually produced as `main.pdf` from `dissertation/main.tex`) and `presentation.pdf` from the `presentation` folder.

**Repository Structure**
- **dissertation/**: Primary thesis source.
	- `main.tex`: Root LaTeX document for the dissertation.
	- `abntex2-modified.cls`, `unbtex.cls`: Local/custom class files used by the thesis.
	- `chapters/`: Individual chapter source files (`1_introduction.tex`, `2_literature_review.tex`, ...).
	- `figures/`: TikZ figures and image assets used in the thesis.
	- `tables/`: LaTeX table fragments and results tables included by chapters.
	- `unbtexcite/`, `unbtexcover/`: Custom bibliography and cover templates/styles.
	- `references/`: BibTeX or bibliography-related files referenced by the thesis.

- **presentation/**: Beamer presentation source and theme files.
	- `presentation.tex`: Root Beamer file for slides.
	- `beamer*.sty`: Local Beamer theme/customization files.

- **README.md**: This file.
- Other files at project root: previously generated PDFs (build artifacts), supplementary files and a `.gitignore`.

**Build / Compile**
To update the dissertation PDFs, it is recommended to run the following commands in a terminal (assuming you have a full TeX distribution installed):

```
cd dissertation
pdflatex main.tex
bibtex main      
makeindex main.nlo -s nomencl.ist -o main.nls
pdflatex main.tex
pdflatex main.tex
```
Or, for the presentation:

```
cd presentation
pdflatex presentation.tex
bibtex presentation
pdflatex presentation.tex
pdflatex presentation.tex
```
