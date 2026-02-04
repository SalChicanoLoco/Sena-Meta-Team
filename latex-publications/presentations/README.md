# Presentations

This directory is for Beamer presentations.

## Usage

1. Copy the presentation template:
   ```bash
   cp -r ../templates/presentation my-presentation-name
   ```

2. Edit `main.tex` to add your slides

3. Add figures if needed

4. Compile:
   ```bash
   cd my-presentation-name
   pdflatex main.tex
   ```

## Organization

Each presentation should be in its own subdirectory with:
- Main Beamer file (main.tex)
- Figures subdirectory (if needed)
- Any supporting files

## Tips

- Keep slides simple with minimal text
- Use one main idea per slide
- Include visuals to support your points
- Practice timing (1-2 minutes per slide)
- Test on projection equipment before presenting
- Consider creating a handout version

## Customization

- Change themes and colors in the preamble
- Adjust aspect ratio (16:9 or 4:3)
- Add animations sparingly with `\pause` or `\only<>`
- Use `\alert{}` to highlight important points
