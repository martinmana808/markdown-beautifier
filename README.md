# Markdown Beautifier 🎨

A premium, browser-based Markdown editor and previewer built with the "Antigravity" design system.

![Markdown Beautifier Preview](./preview.png)

## Features

- **Premium Aesthetics**: Deep slate / cyan theme inspired by modern developer tools.
- **High-Fidelity Typography**: Uses **Fira Code**, **JetBrains Mono**, and **Inter**.
- **Live Preview**: Instant rendering of Markdown to HTML.
- **Developer Experience**:
  - vertical indentation guides.
  - Active line highlighting.
  - Syntax highlighting for code blocks.
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
-   **Editor**: [CodeMirror 5](https://codemirror.net/5/)
-   **Parser**: [Marked.js](https://marked.js.org/)
-   **Icons**: [Lucide](https://lucide.dev/)
-   **Fonts**: Google Fonts (Inter, Fira Code, JetBrains Mono)

## License

ISC
