# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a LaTeX Beamer presentation project about "10 Easy Ways to Contribute to Open Source Projects". The repository contains bilingual presentations (Spanish and English) with a custom presentation class.

## File Structure

- `10-easy-wasy-to-contribute-to-opensource-es.tex` - Spanish version of the presentation
- `10-easy-wasy-to-contribute-to-opensource.tex` - English version of the presentation  
- `presentacion.cls` - Custom LaTeX class file defining the presentation theme and styling
- `img/` - Directory containing presentation images (QR codes, etc.)
- Generated files: `.pdf`, `.aux`, `.log`, `.nav`, `.out`, `.snm`, `.synctex.gz`, `.toc` - LaTeX compilation artifacts

## Build Commands

To build the presentations:

```bash
# Build Spanish version
pdflatex 10-easy-wasy-to-contribute-to-opensource-es.tex

# Build English version  
pdflatex 10-easy-wasy-to-contribute-to-opensource.tex

# For automated building with dependency tracking
latexmk -pdf 10-easy-wasy-to-contribute-to-opensource-es.tex
latexmk -pdf 10-easy-wasy-to-contribute-to-opensource.tex

# Clean build artifacts
latexmk -c
```

## Architecture

The project uses LaTeX Beamer with a custom class:

- **presentacion.cls**: Custom Beamer class that extends the base beamer class with 16:9 aspect ratio, defines custom colors, Font Awesome icon commands, and social text formatting macros
- **Main .tex files**: Use the Madrid theme with seahorse color scheme, include automatic section indexes, and support multilingual content with babel
- **Dependencies**: Requires LaTeX packages including fontawesome, worldflags, tikz, graphicx, epstopdf, and various Beamer extensions

## Key LaTeX Customizations

- Custom frame title templates that use section/subsection headers
- Automatic table of contents at section beginnings
- Font Awesome icon integration for social symbols
- Custom color scheme (basecolor: #0000F0)
- Full-screen PDF mode enabled