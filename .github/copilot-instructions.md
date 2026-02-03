# Copilot / AI Agent instructions for this repository ✅

Short summary
- This repository is a learning collection of **static HTML/CSS** exercises and small projects (see `exercico/`, `desafios/`, `miniProjeto/`). There is no build, bundler, or test framework: pages are previewed directly in a browser.

What an agent should know (high value, actionable items)
1. Project layout
   - `exercico/` = numbered exercises (each exercise is usually self-contained in its own folder). Use `index.html` as the entry file.
   - `desafios/` = challenge folders and answers (e.g., `d010/` package contains `fontes/` and `imagens/`).
   - `miniProjeto/` = slightly larger projects with `index.html`, `style.css`, `fontes/` and `imagens/` subfolders.

2. Previewing and verifying changes ⚙️
   - No build step. To preview: open the relevant `index.html` in a browser or use VS Code Live Server (recommended for quick dev previews).
   - The README links a published preview: https://fernandosampaio-coder.github.io/html-css/exercico — use it to check deployed output after commits.
   - For HTML validation and accessibility checks, use the W3C validator or browser devtools.

3. File & naming conventions to follow
   - Each exercise is typically self-contained: `index.html`, optional `style.css`, `imagens/` and `fontes/` if needed.
   - Use relative paths for assets (e.g., `imagens/xxx.png`, `style.css`). Example: `exercico/ex15/index.html` links `style.css` with `<link rel="stylesheet" href="style.css">`.
   - Keep filenames lowercase and hyphen-separated where possible for consistency. Note: the repo contains mixed naming styles — prefer `kebab-case` for new files.

4. HTML header / boilerplate to reuse (copy/paste)
   - Follow the pattern used across the repo (see `exercico/ex15/index.html` and `miniProjeto/.../android.html`):

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Short descriptive title</title>
  <link rel="stylesheet" href="style.css">
</head>
```

5. Patterns and common techniques used in the codebase
   - Responsive images with `<picture>` and `srcset` are used in mini projects (example: `miniProjeto/miniProjeto1D10HTMLCSS/pacote-projeto-d010/android.html`).
   - Content language is `pt-br` across files — keep `lang="pt-br"` unless intentionally adding English content.
   - Asset folders are typically `imagens/` and `fontes/` inside each project folder.

6. When adding a new exercise or project (practical checklist)
   - Create folder `exNN/` or `desafio-dNN/` (follow existing numbering).
   - Include `index.html` with the boilerplate above, add `style.css` if applicable.
   - Add `imagens/` and `fontes/` subfolders for local assets (update relative paths in HTML/CSS).
   - Preview locally (browser / Live Server) and validate the markup.
   - Commit with a concise message following the local pattern: `ex23: fix table markup` or `miniProj: add responsive images`.

7. What not to change without author confirmation
   - Do not reorganize the entire folder naming scheme (e.g., renaming many exercise directories) without a PR description and agreement — the repo is a learning history and some inconsistencies are intentional.
   - Avoid changing URLs referenced in the README (the published GitHub Pages site) unless you confirm the intended deployment method.

8. Useful files / places to inspect
   - `README.md` (root) — links the published preview.
   - Example exercise: `exercico/ex15/index.html` — canonical header and simple structure.
   - Example mini project: `miniProjeto/miniProjeto1D10HTMLCSS/pacote-projeto-d010/android.html` — demonstrates responsive images, sections, and asset usage.

If something here is unclear or you want me to expand any section (examples, checklists, or add more file links), tell me which part to improve and I'll iterate. 💡
