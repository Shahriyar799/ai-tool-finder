# ToolScout — AI Tool Finder

A lightweight, responsive directory that helps people discover AI products by the task they want to complete.

## What is included

- Responsive single-page website (desktop and mobile).
- Search across tool names, categories and task descriptions.
- Category filters for writing, images, video, coding and research.
- Curated starter directory with direct links to provider websites.
- Basic SEO metadata and accessible page structure.
- No framework, build step, database, API key or server required.

## Run locally

The site is static HTML. Open `index.html` in a browser, or run a small local server:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy

The repository can be deployed as a static site with GitHub Pages or imported into Vercel. No build command is needed; the output directory is the repository root.

### GitHub Pages

1. Open the repository settings.
2. Go to **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select `main` and `/(root)`, then save.
5. GitHub will show the published URL after deployment finishes.

## Editing the directory

The starter catalog lives in the `tools` array near the bottom of `index.html`. Each item has:

- `name`: product name
- `category`: filter category
- `icon`: simple visual symbol
- `tag`: short descriptor
- `desc`: description
- `price`: pricing summary (check provider site before relying on it)
- `url`: official product URL
- `keywords`: words used by the local search

To add a product, add another object to that array. Keep categories consistent with the filter buttons.

## Important

This first version is a static directory and uses a small hand-curated sample catalog. Search runs in the visitor's browser; it is not an AI chatbot and does not call an AI API. Tool details and pricing can change, so verify them before publishing commercial claims. The project is not affiliated with the listed providers.

## License

MIT
