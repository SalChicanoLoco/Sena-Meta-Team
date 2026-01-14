# Thesis Template

This template provides a comprehensive structure for writing a PhD thesis or dissertation.

## Contents

- `main.tex`: Main thesis document with front matter, chapters, and back matter
- `chapters/`: Directory containing chapter files
  - `chapter1.tex`: Introduction
  - `chapter2.tex`: Literature Review
  - `chapter3.tex`: Methodology
  - `chapter4.tex`: Results and Analysis
  - `chapter5.tex`: Conclusion and Future Work
- `references.bib`: BibTeX bibliography file

## Features

- Report document class with professional formatting
- Complete front matter (title page, abstract, declaration, acknowledgments)
- Automatic table of contents, list of figures, and list of tables
- Chapter-based structure with separate files
- Bibliography and appendices
- Headers and footers with page numbers
- Support for mathematical equations, figures, and tables
- Theorem environments

## Usage

1. Copy this template to your working directory:
   ```bash
   cp -r templates/thesis theses/my-thesis
   cd theses/my-thesis
   ```

2. Edit `main.tex` to update metadata (title, author, institution, etc.)

3. Edit chapter files in the `chapters/` directory

4. Add references to `references.bib`

5. Compile the document:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Customization

### Title Page
Update the following in `main.tex`:
- Thesis title
- Author name
- Degree name
- Department
- Institution
- Date

### Chapters
Modify chapter files as needed. Add or remove chapters by:
1. Creating/removing chapter files in `chapters/`
2. Adding/removing `\input{chapters/chapterX}` commands in `main.tex`

### Abstract and Declaration
Customize the abstract and declaration sections in `main.tex`.

### Acknowledgments
Add your acknowledgments in the appropriate section of `main.tex`.

## Tips

- Use consistent naming for chapter files
- Place figures in a `figures/` subdirectory
- Keep each chapter focused on a single topic
- Use `\label{}` and `\ref{}` for cross-references
- Compile multiple times to resolve all references
- Use `\cite{}` for citations
