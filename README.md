# Sena-Meta-Team

A LaTeX publications framework for collaborative academic writing.

## Overview

This repository provides a complete framework for creating and managing LaTeX publications. It includes:

- **Sample LaTeX Template** (`sample.tex`): A comprehensive template demonstrating proper document structure with examples of figures, tables, equations, and citations
- **Bibliography Management** (`references.bib`): Pre-configured BibTeX file with sample references
- **Build Configuration**: Proper `.gitignore` to keep the repository clean from build artifacts

## Getting Started

### Desktop/Laptop Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/SalChicanoLoco/Sena-Meta-Team.git
   cd Sena-Meta-Team
   ```

2. Compile the sample document:
   ```bash
   pdflatex sample.tex
   bibtex sample
   pdflatex sample.tex
   pdflatex sample.tex
   ```

3. Start writing your own publication by modifying `sample.tex` or creating a new `.tex` file based on the template.

### Mobile Git Setup

You can work with this repository directly from your mobile device using Git client apps. Here's how:

#### iOS Setup (Using Working Copy)

[Working Copy](https://workingcopyapp.com/) is a powerful Git client for iOS devices.

1. **Install Working Copy**
   - Download from the App Store (free with in-app purchases for advanced features)

2. **Clone the Repository**
   - Open Working Copy
   - Tap the `+` button in the top-right corner
   - Select "Clone repository"
   - Choose "GitHub" as the source
   - Authenticate with your GitHub account if prompted
   - Search for or enter: `SalChicanoLoco/Sena-Meta-Team`
   - Select the repository and tap "Clone"

3. **Edit LaTeX Files**
   - Navigate to the cloned repository in Working Copy
   - Tap on any `.tex` or `.bib` file to view it
   - Tap "Edit" to modify the file
   - Working Copy has built-in syntax highlighting for LaTeX
   - For advanced editing, use the "Share" button to open files in external editors like:
     - **Textastic**: Professional code editor with LaTeX support
     - **iA Writer**: Markdown and plain text editor
     - **Kodex**: Code editor with syntax highlighting

4. **Commit and Push Changes**
   - After editing, tap "Done" to save changes
   - In the repository view, you'll see modified files marked with an "M"
   - Tap "Commit" at the top
   - Enter a commit message describing your changes
   - Tap "Commit" to save locally
   - Tap "Push" (up arrow) to sync with GitHub
   - Enter your GitHub credentials if prompted

#### Android Setup (Using MGit)

[MGit](https://github.com/maks/MGit) is a free, open-source Git client for Android.

1. **Install MGit**
   - Download from Google Play Store or F-Droid

2. **Clone the Repository**
   - Open MGit
   - Tap the `+` button (bottom-right)
   - Select "Clone repository"
   - Enter repository URL: `https://github.com/SalChicanoLoco/Sena-Meta-Team.git`
   - Choose a local path for the repository
   - If the repository is private, add your GitHub credentials:
     - Tap "Authentication" → "Use account"
     - Enter your GitHub username and personal access token
   - Tap "Clone"

3. **Edit LaTeX Files**
   - In MGit, tap on your repository
   - Navigate to files and tap to view
   - To edit, you'll need an external editor (MGit uses your default text editor)
   - Recommended Android text editors:
     - **Markor**: Excellent for text/markdown editing
     - **QuickEdit**: Fast text editor with syntax highlighting
     - **Acode**: Feature-rich code editor
   - After editing in external app, return to MGit

4. **Commit and Push Changes**
   - In MGit repository view, tap the overflow menu (⋮)
   - Select "Commit"
   - Check the files you want to commit
   - Enter a commit message
   - Tap "Commit"
   - To push: tap overflow menu → "Push" → select remote branch
   - Authenticate if required

#### Android Setup Alternative (Using GitJournal)

[GitJournal](https://gitjournal.io/) is designed for note-taking but works well for text files.

1. **Install GitJournal**
   - Download from Google Play Store or F-Droid

2. **Setup Repository**
   - Open GitJournal
   - Select "Clone Repository"
   - Choose "GitHub" as the provider
   - Authenticate with your GitHub account
   - Select `SalChicanoLoco/Sena-Meta-Team` repository
   - Choose a local folder and clone

3. **Edit and Sync**
   - Browse files in the repository
   - Tap any file to edit
   - GitJournal has a built-in editor with basic features
   - Changes auto-commit and sync based on your settings
   - Or manually sync using the sync button

### Mobile Workflow Tips

1. **Preview LaTeX on Mobile**
   - LaTeX compilation typically requires a desktop environment
   - For previewing, consider:
     - Using Overleaf mobile app (requires uploading files to Overleaf)
     - Using VerbTeX (LaTeX editor for Android with compilation support)
     - Pushing changes and using GitHub Actions for automated compilation
     - Compiling on desktop when needed

2. **Best Practices for Mobile Editing**
   - Make small, focused changes rather than large rewrites
   - Commit frequently with clear messages
   - Pull changes before starting work to avoid conflicts
   - Use a Bluetooth keyboard for extensive editing
   - Preview your changes on desktop when possible

3. **Handling Merge Conflicts on Mobile**
   - Working Copy (iOS) has built-in merge conflict resolution
   - MGit (Android) shows conflicts but requires manual editing
   - For complex conflicts, consider resolving on desktop

4. **Security Tips**
   - Use personal access tokens instead of passwords for HTTPS authentication
   - Generate tokens at: GitHub Settings → Developer settings → Personal access tokens
   - Enable two-factor authentication on your GitHub account
   - Never commit sensitive information to the repository

## LaTeX Template Structure

The `sample.tex` file includes:

- **Title and Author Information**: Customizable title page with multiple author support
- **Abstract**: Brief summary with keywords
- **Sections**: Introduction, Related Work, Methods, Results, Discussion, Conclusion
- **Mathematical Equations**: Examples of inline and displayed equations
- **Tables**: Professional tables using the `booktabs` package
- **Figures**: Figure placement and referencing
- **Citations**: BibTeX citation examples
- **Cross-references**: Automatic numbering for sections, figures, tables, and equations

## Bibliography Management

The `references.bib` file contains sample BibTeX entries for various publication types:

- Books (`@book`)
- Journal articles (`@article`)
- Conference papers (`@inproceedings`)
- Technical reports (`@techreport`)
- Theses (`@phdthesis`, `@mastersthesis`)
- Websites (`@misc`)
- Unpublished works (`@unpublished`)
- Book chapters (`@incollection`)

Add your own references following these examples.

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/your-feature`)
6. Create a Pull Request

## License

This project is open source and available for academic and educational use.

## Support

For issues or questions, please open an issue on GitHub or contact the repository maintainer.