# Common Resources

This directory contains shared resources that can be used across multiple LaTeX documents.

## Files

### macros.tex
Common LaTeX macros and custom commands. Include this in your document with:
```latex
\input{../common/macros}
```

Contains shortcuts for:
- Mathematical notation (sets, linear algebra, calculus)
- Probability and statistics notation
- Complexity classes (Big-O notation)
- Common abbreviations (i.e., e.g., etc., et al.)
- Formatting helpers

### bibliography.bib
Centralized BibTeX bibliography file with example citations. Reference this in your document with:
```latex
\bibliography{../common/bibliography}
```

Contains example entries for:
- Journal articles
- Conference papers
- Books and textbooks
- PhD and Masters theses
- Technical reports
- Websites
- Software

### figures/
Directory for storing shared figures and images that are used across multiple documents.

## Usage

### Using Shared Macros

In your main document, add:
```latex
\input{../common/macros}
```

Then use the macros in your content:
```latex
% Mathematical notation
$x \in \R^n$  % Real numbers
$\norm{x}$    % Vector norm
$\bigO{n^2}$  % Big-O notation

% Abbreviations
\ie           % i.e.
\eg           % e.g.
```

### Using Shared Bibliography

In your main document:
```latex
\bibliographystyle{plain}
\bibliography{../common/bibliography}
```

Then cite entries:
```latex
\cite{knuth1984literate}
\cite{lamport1994latex}
```

### Using Shared Figures

Reference figures from the common directory:
```latex
\includegraphics{../common/figures/diagram.pdf}
```

## Benefits of Shared Resources

1. **Consistency**: Use the same notation and formatting across all documents
2. **Efficiency**: Avoid duplicating common references and macros
3. **Maintainability**: Update shared resources in one place
4. **Collaboration**: Team members use consistent conventions

## Adding New Resources

When adding new shared resources:
1. Place files in the appropriate location (`macros.tex`, `bibliography.bib`, or `figures/`)
2. Document any new macros or commands
3. Ensure file paths work from different document locations
4. Test compilation from multiple document directories
