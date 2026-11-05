# xmas-template

Responsive HTML5 and Bootstrap templates designed for German-language Christmas and holiday-themed landing pages and feature sections.

## Overview

`xmas-template` provides a set of responsive, ready-to-use HTML page templates and components tailored for festive season projects. The templates showcase modular layouts, responsive media loading via `<picture>`, interactive expandable content sections, and dynamically rendered content components powered by vanilla JavaScript.

## Available Templates

### 1. `skeleton.html` (Seitenskelett)
A modular landing page template serving as a comprehensive layout skeleton for holiday content, articles, or gift ideas.
- **Header & Navigation:** Fixed-top Bootstrap navbar with links to various site sections.
- **Card Grid Layout:** Two-column responsive grid layout with content cards covering topics such as Writing, Planning, AI image generation, and Crafts.
- **Static & Dynamic Content:** Demonstrates both static HTML cards and dynamically injected cards generated at runtime via client-side JavaScript (`cardsData`).
- **Interactive Toggles:** Expandable/collapsible content sections ("Mehr anzeigen" / "Weniger anzeigen") with ARIA accessibility states.
- **Responsive Media:** Uses HTML5 `<picture>` tags with responsive breakpoints for adaptive image delivery across desktop and mobile devices.
- **Footer:** Pre-styled section for additional services, company contact info, and legal links.

### 2. `playlist.html` (Festliche Klänge)
A Christmas music playlist interface designed with an elegant festive color palette (dark midnight blue, light ice blue, and rich gold accents).
- **Hero & Header:** Curated festive banner section with typography powered by Google Fonts (*Spline Sans*, *Noto Sans*, and *Playfair Display*).
- **Dynamic Track List:** Renders an interactive list of classic Christmas songs and descriptions injected via client-side JavaScript.
- **Custom UI Components:** SVG music icons, interactive navigation buttons, and responsive item cards.

## Repository Structure

```text
xmas-template/
├── css/
│   ├── bootstrap.min.css     # Bootstrap core stylesheet
│   └── localstyle.css        # Custom styles and utility classes
├── js/
│   └── bootstrap.bundle.min.js # Bootstrap bundled JavaScript (with Popper)
├── playlist.html             # Christmas playlist template
├── skeleton.html             # Modular landing page skeleton template
├── whatis.md                 # German description & documentation of skeleton.html
└── README.md                 # Project documentation
```

## Technologies & Dependencies

- **HTML5 & CSS3:** Semantic markup, CSS custom properties (variables), responsive media queries, and flexbox layouts.
- **Bootstrap (v4):** Grid system, navigation components, cards, and responsive utilities.
- **JavaScript:** Pure Vanilla JavaScript for DOM manipulation, dynamic component rendering, and UI toggles; jQuery Slim for Bootstrap components.
- **Typography:** Google Fonts integration (*Spline Sans*, *Noto Sans*, *Playfair Display*).
- **Image Assets:** Placeholder images provided via `via.placeholder.com` for easy replacement.

## Getting Started & Local Preview

No build step or package manager installation is required. You can preview and run the templates directly in any modern web browser.

### Option 1: Direct File Access
Simply open the HTML files directly in your web browser:
- Double-click `skeleton.html` or `playlist.html` in your file manager, or
- Drag and drop the file into an open browser window.

### Option 2: Local Static Server
If you prefer running a local HTTP server:

Using Python 3:
```bash
python3 -m http.server 8000
```
Then navigate to `http://localhost:8000/skeleton.html` or `http://localhost:8000/playlist.html` in your browser.

Using Node.js (`npx serve` or `http-server`):
```bash
npx serve .
```

## Customization Guide

### Updating Content & Data
- **Dynamic Cards in `skeleton.html`:** Edit the `cardsData` array in the inline `<script>` tag at the bottom of `skeleton.html` to modify image sources, titles, descriptions, and bullet items.
- **Playlist Tracks in `playlist.html`:** Edit the `playlistData` array in `playlist.html` to add, remove, or modify song titles and descriptions.

### Replacing Images
Replace `https://via.placeholder.com/...` image URLs in `skeleton.html` and `playlist.html` with your actual image paths or external CDN links. Remember to update the `alt` attributes and photo credits accordingly.

### Custom Styling
- Global styles and color overrides can be placed in `css/localstyle.css`.
- Page-specific styles and CSS variable definitions (`--rich-gold`, `--dark-blue-bg`, etc.) are located within the `<style>` blocks in the `<head>` of each template.
