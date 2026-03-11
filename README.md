# de-bug-duck

de-bug-duck is a small static web app that acts like a virtual debugging rubber duck.

## Run Locally

Because this project is static HTML/CSS/JS, you can serve it with any static file server.

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy To Render (Static Site)

This repository includes a `render.yaml` blueprint configured for Render static-site deployment.

### Option 1: Blueprint Deploy (recommended)

1. Push this repository to GitHub.
2. In Render, click `New +` -> `Blueprint`.
3. Select this repository.
4. Render will detect `render.yaml` and create the static site.

### Option 2: Manual Static Site Setup

1. In Render, click `New +` -> `Static Site`.
2. Connect this repository.
3. Use these values:
	- Build Command: *(leave empty)*
	- Publish Directory: `.`

## Notes

- Main entry file: `index.html`
- Static assets: `static/`
- No backend runtime is required.
