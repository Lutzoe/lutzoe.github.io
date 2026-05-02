# Temporal Graph Atlas (TGA)

[![Build Status](https://github.com/tgatlas/temporal-graphs-atlas.github.io/workflows/CI%2FCD%20Pipeline/badge.svg)](https://github.com/tgatlas/temporal-graphs-atlas.github.io/actions)
[![Website](https://img.shields.io/website?url=https%3A%2F%2Ftemporal-graphs-atlas.github.io)](https://temporal-graphs-atlas.github.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A comprehensive, community-driven resource for research on **Temporal Graphs** -
maintaining an overview of the current state of research and collecting links to relevant materials
to help researchers navigate this rapidly growing field.

## Mission

The idea of this project is to maintain an overview over the current state of research on Temporal
Graphs and collect links to further relevant material. This should especially help new researchers
in this field to orient faster, but we also try to keep track over and cluster the large amount of
results and publications in this field.

## How to Contribute in General

The sources and data for this webpage are available on
[GitHub](https://github.com/tgatlas/temporal-graphs-atlas.github.io). It uses
[Vite](https://vitejs.dev/) + [React 19](https://react.dev/) to build a static site and is hosted
via [GitHub Pages](https://pages.github.com/).

Everyone is very welcome to contribute:

- Maintain paper references, e.g. adding, updating and labeling references (see `papers/` directory
  and syntax below)
- Add and edit further material. Key Markdown sources live in `public/content/`:
  - `public/content/material.md` (Material page)
  - `public/content/about.md` (About page)
  - `public/content/contribute.md` (Contribute page)
- Improve layout or design, add new features.

Most contributions can be done via Pull Requests directly in the repository. For more involved
suggestions or discussions, feel free to open an issue on GitHub.

## Adding and Editing Paper References

Paper entries are based on YAML files, which are located in the directory `papers/`.

As an example, this is a data file for a temporal graph paper (`Author21topic.yml`):

```yml
title: Paper Title on Temporal Graphs
authors: Author1, Author2
publications:
  - name: STOC
    year: 2021
    url: https://example.com/paper.pdf
  - name: arXiv
    year: 2021
    month: 3
    url: https://arxiv.org/abs/2101.12345
labels:
  - connectivity
  - temporal paths
```

If you want to add or change the entry of a paper, you can either add/edit the file via a Pull
Request or open an issue on GitHub. In case you want to add a paper, please try to find a unique
filename (as in the example above; but there are no strict conventions).

## Local Development

Prerequisites: Node.js >= 18 and npm >= 8.

First, clone
[this repository](https://github.com/tgatlas/temporal-graphs-atlas.github.io)
and install dependencies via npm:

```bash
npm install
```

Then start the development server:

```bash
npm run dev
```

The site will be available at `http://localhost:3000`.

## 🛠️ Technology Stack

- **Build Tool**: [Vite 6](https://vitejs.dev/)
- **Framework**: [React 19](https://react.dev/)
- **UI Library**: [Material-UI (MUI) v7](https://mui.com/)
- **Styling**: [Emotion](https://emotion.sh/)
- **Content**: Markdown files in `public/content/*.md`
- **Data Processing**: Node.js scripts for YAML and JSON generation (`scripts/`)
- **Code Quality**: ESLint, Prettier, Husky for git hooks
- **CI/CD**: GitHub Actions for automated testing and deployment
- **Hosting**: GitHub Pages with automated deployments

## 📊 Project Scripts

```bash
npm run dev             # Compose data and start Vite dev server
npm run start           # Alias for dev
npm run build           # Compose data and build production site
npm run preview         # Preview the built site locally
npm run format          # Format code with Prettier
npm run format:check    # Check formatting without writing
npm run lint            # Run ESLint checks
npm run lint:fix        # Fix lint issues automatically
npm run clean           # Clean build cache (dist and Vite cache)
npm run clean:all       # Remove dist, node_modules, and lockfile
npm run deploy          # Deploy to GitHub Pages (branch: deploy)
npm run test            # Run tests with Vitest
npm run test:coverage   # Run tests with coverage report
npm run test:ui         # Run tests with UI
```

## 🤝 Contributing

We welcome contributions from the community! See our
[How to Contribute](https://temporal-graphs-atlas.github.io/contribute) page for detailed
guidelines.
