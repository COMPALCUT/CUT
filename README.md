# Manufacturing Engineering Knowledge Base

A Confluence-style engineering knowledge base built with **MkDocs Material** and hosted using **GitHub Pages**.

## What is included

- Home dashboard
- Process Engineering section
- NPI section
- Equipment documentation
- Server platform pages
- Forms and reusable engineering templates
- Mermaid process-flow support
- Search
- Dark/light mode
- Automatic GitHub Pages deployment

## First-time setup

1. Create a GitHub repository named `engineering-wiki`.
2. Upload all files and folders from this starter repository.
3. Edit `mkdocs.yml` and replace `YOUR-USERNAME` with your GitHub username.
4. Commit/push to the `main` branch.
5. In GitHub, open **Settings > Pages**.
6. Under **Build and deployment**, select **Deploy from a branch**.
7. Select branch `gh-pages` and folder `/ (root)` after the workflow has run once.
8. Your documentation site will be available at:

   `https://YOUR-USERNAME.github.io/engineering-wiki/`

## Local preview (optional)

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve
```

Then open the local address shown in the terminal.

## Editing content

Most documentation is stored under `docs/` as Markdown (`.md`) files. You can edit them directly in GitHub using the pencil icon, so contributors do not need to install anything.
