# APEC Lab Website Project

## Project Overview

This project contains the source code for **The APEC Lab** website (Assessment, Planning, Ecology, Conservation?). It is a static site built using **Hugo**, specifically utilizing the **Wowchemy (now Hugo Blox)** Research Group template.

The site is designed to showcase the research group's:
*   Members (`content/en/authors/`)
*   Publications (`content/en/publication/`)
*   Events (`content/en/event/`)
*   Research Projects (`content/en/research/`)
*   Blog Posts (`content/en/post/`)

## Prerequisites

To work on this project, you need:

*   **Hugo:** A static site generator. The `netlify.toml` specifies `HUGO_VERSION = "0.135.0"`. It is recommended to use the "extended" version of Hugo for SCSS/SASS support.
*   **Go:** Required for managing Hugo Modules (dependencies).

## Building and Running

### Local Development

To run the site locally with live reloading:

```bash
hugo server
```

By default, the site will be available at `http://localhost:1313`.

### Production Build

To build the static files for production (output to `public/` directory):

```bash
hugo --gc --minify
```

### Dependency Management

This project uses Hugo Modules. To update the theme/modules:

```bash
hugo mod get -u
hugo mod tidy
```

## Project Structure

*   **`config/_default/`**: Main configuration files (`hugo.yaml`, `menus.yaml`, `params.yaml`).
*   **`content/en/`**: The website content.
    *   `authors/`: Individual profiles for group members.
    *   `publication/`: Bibliographic entries for publications.
    *   `post/`: News and blog posts.
*   **`assets/`**: Source assets.
    *   `scss/`: Custom CSS styling (`custom.scss`).
    *   `media/`: Images and media files.
*   **`static/`**: Static files served directly (e.g., large files, `uploads`, `video`).
*   **`layouts/`**: HTML templates for overriding the theme's default layout.
*   **`netlify.toml`**: Configuration for deployment on Netlify.
*   **`go.mod` / `go.sum`**: Go module definitions for Hugo dependencies.

## Key Conventions

*   **Content:** Written in Markdown (mostly `.md` files). Front matter is typically in YAML.
*   **Citations:** Publications can be imported or managed via `cite.bib` files in their respective folders.
*   **Styling:** Use `assets/scss/custom.scss` for style overrides to ensure they persist after theme updates.
