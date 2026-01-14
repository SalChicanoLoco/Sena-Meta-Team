# Academic Paper Template

This template provides a starting point for writing academic research papers.

## Contents

- `main.tex`: Main LaTeX document with complete structure
- `references.bib`: BibTeX bibliography file with example citations

## Features

- Standard article class with professional formatting
- Common packages for scientific writing
- Math support (equations, theorems, proofs)
- Figure and table support
- Bibliography management with BibTeX
- Algorithm pseudocode support
- Code listing support
- Hyperlinked references and citations

## Usage

1. Copy this template to your working directory:
   ```bash
   cp -r templates/academic-paper papers/my-paper
   cd papers/my-paper
   ```

2. Edit `main.tex` to add your content

3. Add your references to `references.bib`

4. Compile the document:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Customization

### Document Metadata
Update the following in `main.tex`:
- Title
- Author information
- Date
- Keywords

### Sections
Modify sections according to your needs. Common sections include:
- Introduction
- Related Work
- Methodology
- Results
- Discussion
- Conclusion

### Packages
The template includes commonly used packages. Add or remove packages based on your requirements.

## Tips

- Use `\label{}` and `\ref{}` for cross-references
- Place figures in a `figures/` subdirectory
- Use `\cite{}` for citations
- Run BibTeX after adding new citations
- Use `\todo{}` command to mark items needing attention (appears in red)
