# surveydown Workshop Website

This is a Quarto website for a workshop on using [surveydown](https://surveydown.org/) to build reproducible and programmable surveys.

## Project Overview

This workshop teaches participants how to create surveys using the surveydown platform, which is an R package that combines Quarto and Shiny to create dynamic, programmable surveys.

**Workshop Instructor**: Dr. John Paul Helveston (jph@gwu.edu)

**Website URL**: https://jhelvy.github.io/2025-qux-surveydown-workshop/

## Project Structure

### Main Files

- `index.qmd` - Homepage with workshop overview and navigation cards
- `install.qmd` - Installation instructions for surveydown
- `LICENSE.qmd` - License information (CC-BY-SA)
- `_quarto.yml` - Main Quarto configuration file
- `styles.css` & `theme.scss` - Custom styling
- `examples.zip` - Downloadable examples for participants

### Workshop Content

The workshop is organized into 4 parts (located in `parts/` directory):

1. **Getting Started** (`parts/getting-started.html`) - Learn the basic structure of a surveydown survey and create your first survey
2. **Conditional Control** (`parts/conditional-control.html`) - Take control over page navigation and content display based on question responses
3. **Data Handling** (`parts/data-handling.html`) - Set up your database to store response data and dynamically use the data in your survey
4. **Reactivity** (`parts/reactivity.html`) - Leverage Shiny's powerful reactivity framework to make surveys more dynamic

### Other Directories

- `_site/` - Generated website output (do not edit directly)
- `_extensions/` - Quarto extensions
- `_includes/` - HTML includes for the website
- `fragments/` - Reusable content fragments (not rendered as standalone pages)
- `.github/` - GitHub Actions and workflows

## Development

### Building the Site

To preview the website locally:
```bash
quarto preview
```

The site runs on port 5896 by default (configured in `_quarto.yml`).

To render the full site:
```bash
quarto render
```

Or use the R script:
```bash
Rscript render.R
```

### Key Configuration Notes

- The site uses the Flatly theme with custom SCSS (`theme.scss`)
- Search is disabled in the navbar
- The site includes Font Awesome icons for navigation
- Code linking is enabled for better reference

## About surveydown

surveydown is an R package for building surveys using:
- **Quarto** for creating markdown-based survey content
- **Shiny** for reactivity and dynamic behavior
- **Database integration** for storing responses

For more information, visit [surveydown.org](https://surveydown.org/).

## License

This workshop content is licensed under CC-BY-SA (Creative Commons Attribution-ShareAlike).
