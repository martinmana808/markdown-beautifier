# GEMINI.md (The Index)

## Project Summary
**Markdown Beautifier** is a premium, single-page web application designed to render raw Markdown into highly aesthetic documents using the Antigravity design system.

## Tech Stack
-   **Frontend:** HTML5, Vanilla CSS, JavaScript.
-   **Libraries:** Marked.js (Markdown parsing), Highlight.js, Lucide Icons.
-   **Design:** Custom "Antigravity" tokens, Inter/Fira Code typography.

## History


### [2026-02-18] Yellow Highlighting (< CONTENT > and ++) | [log-20260218-yellow-highlighting](./GEMINI--logs.md#log-20260218-yellow-highlighting)
-   Implemented yellow highlighting for text contained within `< >` bubbles.
-   Synchronized the `++` whole-line rule to use the same yellow color (#DFC184).




### [2026-02-18] View Modes (RAW, LIVE, HYBRID) | [log-20260218-view-modes](./GEMINI--logs.md#log-20260218-view-modes)
-   Implemented a view mode switcher in the header.
-   Options: RAW (Editor only), LIVE (Preview only), HYBRID (Split screen).
-   Set RAW as the default view and persisted preference in `localStorage`.

### [2026-02-18] Plus (++) Highlighting | [log-20260218-plus-rule](./GEMINI--logs.md#log-20260218-plus-rule)
-   Implemented a new orange highlighting rule for lines containing `++`.
-   Prioritized the rule to ensure it captures the whole line as intended.

### [2026-02-18] Visual Indentation Tabs | [log-20260218-visual-tabs](./GEMINI--logs.md#log-20260218-visual-tabs)
-   Implemented a space-to-tab conversion rule in the custom highlighter.
-   Replaces every pair of spaces with a `.tab` span featuring a vertical border guide.
-   Ensured the logic is cumulative and compatible with tiered hyphens.

### [2026-02-18] Tiered Hyphen Highlighting | [log-20260218-tiered-hyphens](./GEMINI--logs.md#log-20260218-tiered-hyphens)
-   Implemented hierarchical hyphen highlighting (1, 2, or 3 hyphens).
-   Each level colors the entire line with progressively darker shades of white/grey (monochrome).
-   Refined Level 2 and Level 3 to appear as a single hyphen by hiding sacrificial characters (`opacity:0`, `font-size:0`).
-   Ensured lines with more than 3 hyphens (separators) remain uncolored.
-   Enhanced prefix logic to allow highlighting after spaces or brackets (e.g. `(--` or `(---`).

### [2026-02-18] Custom Syntax Highlighter | [log-20260218-custom-syntax](./GEMINI--logs.md#log-20260218-custom-syntax)
-   Implemented a custom "Ghost Editor" (layered textarea + div) for editor syntax highlighting.
-   Built a regex engine to apply specific user-defined color rules (multiline `*`, `<!-- -->`, etc.).
-   Ensured perfect scroll and text alignment between input and display layers.
-   Replaced standard textarea with this high-performance custom highlighter.

### [2026-02-18] CodeMirror Integration Removal | [log-20260218-remove-codemirror](./GEMINI--logs.md#log-20260218-remove-codemirror)
-   Completely removed CodeMirror scripts, styles, and initialization logic.
-   Restored a standard, styled `textarea` for markdown input.
-   Implemented custom Tab key handling for the textarea.
-   Maintained rendering integration and copy button functionality.

### [2026-02-18] Aesthetic Alignment Refinement | [log-20260218-aesthetic-refinement](./GEMINI--logs.md#log-20260218-aesthetic-refinement)
-   Refined preview colors to match Antigravity (Gemini) rendering exactly.
-   Applied specific colors to headers (H1: Red, H2: Orange, H3: Violet, H4: Green).
-   Adjusted background contrast and fine-tuned blockquote/hr styles.

### [2026-02-18] Antigravity Rendering Alignment | [log-20260218-antigravity-rendering](./GEMINI--logs.md#log-20260218-antigravity-rendering)
-   Integrated `highlight.js` and enhanced GFM alerts with Lucide icons.
-   Added language headers and copy buttons to code blocks.
-   Refined typography and table styles for premium "Antigravity" look.

### [2026-02-05] Project Documentation | [log-20260205-readme](./GEMINI--logs.md#log-20260205-readme)
-   Added comprehensive `README.md`.

### [2026-02-05] Indentation Guides | [log-20260205-indent-guides](./GEMINI--logs.md#log-20260205-indent-guides)
-   Added vertical indentation lines to the editor.

### [2026-02-05] Font Update & DX Fix | [log-20260205-font-update](./GEMINI--logs.md#log-20260205-font-update)
-   Switched editor font to Fira Code / Consolas.
-   Added `package.json` for `npm run dev` support.

### [2026-02-05] Reskin Left Panel Editor | [log-20260205-reskin-editor](./GEMINI--logs.md#log-20260205-reskin-editor)
-   Refined Left Panel (Markdown Editor) with premium dark theme.
-   Added active line highlighting and transparent backgrounds.

### [2026-01-20] Initial Project Sync | [log-20260120-initial-sync](./GEMINI--logs.md#log-20260120-initial-sync)
-   Project initialized and structured with GEMINI logging protocol.
-   Git repository initialized and linked to GitHub.
-   Baseline `index.html` reviewed and confirmed operational.

---
*Created by Antigravity AI.*
