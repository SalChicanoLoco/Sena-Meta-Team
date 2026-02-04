# LaTeX Publications Repository

This directory contains LaTeX templates and resources for academic publications, including research papers, theses, and presentations.

## Directory Structure

```
latex-publications/
├── templates/          # Template files for different document types
├── papers/            # Research papers and articles
├── theses/            # Thesis and dissertation documents
├── presentations/     # Beamer presentations
└── common/            # Shared resources (bibliography, images, etc.)
```

## Getting Started

### Prerequisites

You need a LaTeX distribution installed on your system:

- **Linux**: Install TeX Live
  ```bash
  sudo apt-get install texlive-full
  ```

- **macOS**: Install MacTeX
  ```bash
  brew install --cask mactex
  ```

- **Windows**: Install MiKTeX or TeX Live
  - Download from [MiKTeX](https://miktex.org/) or [TeX Live](https://www.tug.org/texlive/)

### Compiling Documents

#### Method 1: Using pdflatex (recommended)
```bash
cd latex-publications/papers/your-paper
pdflatex main.tex
bibtex main      # if using bibliography
pdflatex main.tex
pdflatex main.tex
```

#### Method 2: Using latexmk (automated)
```bash
cd latex-publications/papers/your-paper
latexmk -pdf main.tex
```

#### Method 3: Using XeLaTeX (for advanced fonts)
```bash
cd latex-publications/papers/your-paper
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

## Templates

### Academic Paper Template
Located in `templates/academic-paper/`, this template includes:
- Standard article structure
- Bibliography support
- Common packages for scientific writing
- Proper formatting for equations and figures

### Thesis Template
Located in `templates/thesis/`, this template provides:
- Chapter-based structure
- Table of contents, list of figures, list of tables
- Bibliography and appendices
- Customizable front matter

### Presentation Template
Located in `templates/presentation/`, this Beamer template offers:
- Professional slide layouts
- Title slide, content slides, and reference slide
- Customizable themes and colors

## Common Resources

The `common/` directory contains shared resources:
- `bibliography.bib`: Centralized BibTeX bibliography file
- `macros.tex`: Common LaTeX macros and custom commands
- `figures/`: Shared images and figures

## Usage Guide

### Creating a New Paper

1. Copy the academic paper template:
   ```bash
   cp -r templates/academic-paper papers/my-new-paper
   cd papers/my-new-paper
   ```

2. Edit `main.tex` with your content

3. Add references to `references.bib`

4. Compile:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

### Creating a New Presentation

1. Copy the presentation template:
   ```bash
   cp -r templates/presentation presentations/my-talk
   cd presentations/my-talk
   ```

2. Edit `main.tex` with your slides

3. Compile:
   ```bash
   pdflatex main.tex
   ```

## Tips and Best Practices

1. **Version Control**: Commit your `.tex` files but not the generated PDFs or auxiliary files (handled by `.gitignore`)

2. **Bibliography Management**: Use a reference manager like Zotero, Mendeley, or JabRef to maintain your BibTeX files

3. **Collaborative Writing**: Consider using Overleaf for real-time collaboration, then sync back to this repository

4. **Figure Management**: Store figures in a dedicated `figures/` subdirectory within each project

5. **Modular Documents**: For large documents, split content into separate `.tex` files and use `\input{}` or `\include{}`

## Useful Resources

- [LaTeX Wikibook](https://en.wikibooks.org/wiki/LaTeX)
- [Overleaf Documentation](https://www.overleaf.com/learn)
- [CTAN - Comprehensive TeX Archive Network](https://ctan.org/)
- [TeX Stack Exchange](https://tex.stackexchange.com/)

## Common Issues

### Missing Packages
If you encounter missing package errors, install them:
```bash
# Ubuntu/Debian
sudo apt-get install texlive-<package-name>

# Or use tlmgr
tlmgr install <package-name>
```

### Bibliography Not Appearing
Make sure to run the compilation sequence:
```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

### Font Issues
For special fonts, use XeLaTeX or LuaLaTeX instead of pdflatex.

## Contributing

When adding new templates or examples:
1. Place them in the appropriate directory
2. Include a README in the template directory
3. Document any special requirements or packages
4. Test compilation before committing
