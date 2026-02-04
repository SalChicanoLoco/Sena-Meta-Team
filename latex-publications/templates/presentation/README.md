# Presentation Template (Beamer)

This template provides a structure for creating academic presentations using LaTeX Beamer.

## Contents

- `main.tex`: Main Beamer presentation document

## Features

- Modern Madrid theme with customizable colors
- Structured sections for a complete presentation
- Title slide with institutional information
- Automatic outline/table of contents
- Support for columns, blocks, and mathematical equations
- Figure and table support
- Footer with author, title, and page numbers
- Thank you and references slides

## Usage

1. Copy this template to your working directory:
   ```bash
   cp -r templates/presentation presentations/my-talk
   cd presentations/my-talk
   ```

2. Edit `main.tex` to add your content:
   - Update title, author, and institution
   - Modify or add slides
   - Add your figures

3. Compile the presentation:
   ```bash
   pdflatex main.tex
   ```

## Customization

### Theme and Colors
Change the theme and color scheme by modifying:
```latex
\usetheme{Madrid}        % Try: Berlin, Copenhagen, Warsaw, etc.
\usecolortheme{default}  % Try: dolphin, seagull, rose, etc.
```

Or define custom colors:
```latex
\definecolor{myblue}{RGB}{0,82,155}
\setbeamercolor{structure}{fg=myblue}
```

### Aspect Ratio
The template uses 16:9 aspect ratio by default. For 4:3, change:
```latex
\documentclass[aspectratio=169]{beamer}  % 16:9
\documentclass[aspectratio=43]{beamer}   % 4:3
```

### Slide Layout
Common slide layouts:
- **Two columns**: Use `\begin{columns}...\end{columns}`
- **Blocks**: Use `\begin{block}{Title}...\end{block}`
- **Lists**: Use `itemize`, `enumerate`, or `description`
- **Math**: Use `equation` or inline math with `$...$`

## Slide Organization

The template includes:
1. **Title slide**: Automatic title page
2. **Outline**: Table of contents
3. **Introduction**: Problem and motivation
4. **Background**: Related work and context
5. **Methodology**: Your approach
6. **Results**: Experimental findings
7. **Conclusion**: Summary and future work
8. **Thank you slide**: Contact information
9. **References**: Bibliography (optional)

## Tips

- Keep slides simple with minimal text
- Use bullet points instead of paragraphs
- Include visuals (figures, charts, diagrams)
- One main idea per slide
- Use animations sparingly
- Practice timing (typically 1-2 minutes per slide)
- Test your presentation on the projection equipment

## Useful Commands

- `\pause`: Reveal content incrementally
- `\alert{text}`: Highlight important text
- `\textbf{text}`: Bold text
- `\textit{text}`: Italic text
- `\only<2>{content}`: Show content only on slide 2
- `\onslide<2->{content}`: Show content from slide 2 onwards
