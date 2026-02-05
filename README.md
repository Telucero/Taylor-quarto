# Taylor's Portfolio - Quarto Static Site

A personal portfolio website built with Quarto, showcasing GitHub projects, technical articles, and other information.

## Features

- **Homepage**: Welcome page with overview of the site
- **Projects**: Showcase of GitHub repositories and other projects
- **Articles**: Technical articles, tutorials, and interesting information
- **About**: Personal information and background
- **Responsive Design**: Clean, professional theme with custom styling

## Prerequisites

- [Quarto](https://quarto.org/docs/get-started/) installed on your system

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Telucero/Taylor-quarto.git
   cd Taylor-quarto
   ```

2. Install Quarto if you haven't already:
   - Visit [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
   - Download and install the appropriate version for your operating system

## Building the Site

To preview the site locally:

```bash
quarto preview
```

This will start a local server and open the site in your browser. The site will automatically reload when you make changes.

To build the site for production:

```bash
quarto render
```

The generated site will be in the `_site/` directory.

## Publishing

### GitHub Pages (Automatic)

This repository includes a GitHub Actions workflow that automatically builds and deploys the site to GitHub Pages when changes are pushed to the `main` or feature branches.

To enable GitHub Pages:
1. Go to your repository Settings > Pages
2. Under "Build and deployment", select "GitHub Actions" as the source
3. Push your changes to trigger the workflow

The workflow will:
- Install Quarto
- Build the site
- Deploy to GitHub Pages

### Manual Publishing

To manually publish to GitHub Pages:

```bash
quarto publish gh-pages
```

### Other Platforms

The `_site/` directory contains the complete static website that can be deployed to any static hosting service:
- Netlify
- Vercel
- AWS S3
- Any web server

## Project Structure

```
Taylor-quarto/
├── _quarto.yml         # Quarto configuration
├── index.qmd           # Homepage
├── projects.qmd        # Projects showcase
├── articles.qmd        # Articles and information
├── about.qmd           # About page
├── styles.css          # Custom CSS styles
├── .gitignore          # Git ignore file
└── README.md           # This file
```

## Customization

- Edit `_quarto.yml` to change site configuration, theme, and navigation
- Modify `.qmd` files to update page content
- Update `styles.css` to customize the appearance
- Add new pages by creating new `.qmd` files and adding them to the navbar in `_quarto.yml`

## License

This project is open source and available under the MIT License.

## Built With

- [Quarto](https://quarto.org) - Scientific and technical publishing system
- Markdown - Content writing
- CSS - Custom styling

## Contact

- GitHub: [@Telucero](https://github.com/Telucero)
- Repository: [Taylor-quarto](https://github.com/Telucero/Taylor-quarto)