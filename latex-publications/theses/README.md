# Theses

This directory is for thesis and dissertation documents.

## Usage

1. Copy the thesis template:
   ```bash
   cp -r ../templates/thesis my-thesis-name
   ```

2. Edit `main.tex` to update metadata

3. Edit chapter files in the `chapters/` directory

4. Add references to `references.bib`

5. Compile:
   ```bash
   cd my-thesis-name
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Organization

Each thesis should be in its own subdirectory with:
- Main LaTeX file (main.tex)
- Chapters directory with individual chapter files
- Bibliography file (references.bib)
- Figures directory
- Any supporting materials

## Tips

- Keep each chapter in a separate file for easier management
- Use consistent naming for chapter files (chapter1.tex, chapter2.tex, etc.)
- Regularly backup your work
- Compile frequently to catch errors early
- Use version control (Git) to track changes
