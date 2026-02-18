# Markdown Beautifier 🎨

A premium, browser-based Markdown editor and previewer built with the "Antigravity" design system.

![Markdown Beautifier Preview](./preview.png)

## Features

- **Premium Aesthetics**: Deep slate / cyan theme inspired by modern developer tools.
- **High-Fidelity Typography**: Uses **Fira Code**, **JetBrains Mono**, and **Inter**.
- **Ghost Editor**: A custom-built, layered syntax highlighter with:
  - **Hierarchical Hyphens**: 1, 2, or 3 hyphens color-coded with visual "single bullet" collapsing.
  - **Yellow Highlighting**: Automatic yellow marking for `< CONTENT >` and `++` lines.
  - **Visual Indentation**: Seamless vertical guides using `.tab` spans.
- **View Modes**: Toggle between **RAW** (Highlighter), **LIVE** (Preview), and **HYBRID** (Split).
- **GitHub Alerts**: Support for `[!NOTE]`, `[!TIP]`, `[!WARNING]`, and `[!IMPORTANT]`.
- **Export**: Copy HTML or Print to PDF.

## Usage

### Local Development

This project is a static single-page application (SPA), but for the best experience (and to avoid CORS issues with local files), use the included dev server:

1.  Install dependencies (optional, for `serve`):
    ```bash
    npm install
    ```

2.  Start the dev server:
    ```bash
    npm run dev
    # or
    npx serve .
    ```

3.  Open `http://localhost:3000` (or whatever port `serve` assigns).

## Tech Stack

-   **Core**: HTML5, Vanilla CSS, JavaScript
-   **Editor**: Custom "Ghost Editor" (Layered Textarea + CSS Highlighter)
-   **Parser**: [Marked.js](https://marked.js.org/)
-   **Icons**: [Lucide](https://lucide.dev/)
-   **Fonts**: Google Fonts (Inter, Fira Code, JetBrains Mono)

## License

ISC
