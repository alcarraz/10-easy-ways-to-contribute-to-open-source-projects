# 10 Easy Ways to Contribute to Open Source Projects

A bilingual presentation (Spanish/English) about accessible ways to contribute to open source projects, featuring real-world examples and practical guidance for new contributors.

## Overview

This presentation covers 10 practical approaches that anyone can use to start contributing to open source projects, regardless of their technical background or experience level. The content is designed to encourage participation in the open source community by showing concrete, achievable ways to make meaningful contributions.

## Available Versions

- **Spanish**: `10-easy-wasy-to-contribute-to-opensource-es.tex`
- **English**: `10-easy-wasy-to-contribute-to-opensource.tex`

## Prerequisites

To build the presentations, you need:

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Required packages: `beamer`, `fontawesome`, `worldflags`, `tikz`, `babel`

## Building the Presentations

### Using pdflatex

```bash
# Build Spanish version
pdflatex 10-easy-wasy-to-contribute-to-opensource-es.tex

# Build English version  
pdflatex 10-easy-wasy-to-contribute-to-opensource.tex
```

### Using latexmk (recommended)

```bash
# Build Spanish version with automatic dependency handling
latexmk -pdf 10-easy-wasy-to-contribute-to-opensource-es.tex

# Build English version
latexmk -pdf 10-easy-wasy-to-contribute-to-opensource.tex

# Build both versions
latexmk -pdf *.tex
```

### Cleaning build artifacts

```bash
latexmk -c
```

## Presentation Features

- Custom Beamer theme based on Madrid with seahorse colors
- 16:9 aspect ratio optimized for modern displays
- Automatic section navigation with table of contents
- Font Awesome icons for enhanced visual elements
- Full-screen presentation mode enabled
- Bilingual support with proper language settings

## File Structure

```
├── 10-easy-wasy-to-contribute-to-opensource-es.tex    # Spanish presentation
├── 10-easy-wasy-to-contribute-to-opensource.tex       # English presentation
├── presentacion.cls                                    # Custom LaTeX class
├── img/                                               # Images and assets
│   └── qr-code.png
└── README.md                                          # This file
```

## Author

**Andrés Alcarraz**

- 📧 Email: [alcarraz@gmail.com](mailto:alcarraz@gmail.com)
- 💼 LinkedIn: [linkedin.com/in/andresalcarraz](https://www.linkedin.com/in/andresalcarraz)
- 🐙 GitHub: [github.com/alcarraz](https://www.github.com/alcarraz)
- 🐦 X (Twitter): [@andresalcarraz](https://x.com/users/andresalcarraz)

## License

This presentation is available for educational and community use.