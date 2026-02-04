# Papers

This directory is for your research papers and articles.

## Usage

1. Copy a template:
   ```bash
   cp -r ../templates/academic-paper my-paper-name
   ```

2. Edit the paper content in `main.tex`

3. Add references to `references.bib`

4. Compile:
   ```bash
   cd my-paper-name
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Organization

Each paper should be in its own subdirectory with:
- LaTeX source files (.tex)
- Bibliography file (.bib)
- Figures subdirectory (if needed)
- README with paper-specific notes

## Tips

- Use descriptive directory names (e.g., `quantum-algorithm-2024`)
- Keep paper-specific figures in the paper's directory
- Use the common bibliography for shared references
- Document any special compilation requirements in a README
