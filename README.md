# GROVE One-page Plan

Internal strategy page for GROVE —
AI-powered Knowledge Layer for frontline teams.

Static site, no framework runtime, no backend. Built with [Vite](https://vitejs.dev) purely as a dev server / bundler for a plain HTML page.

## Development

```
npm install
npm run dev
```

Opens a local dev server (default `http://localhost:5173`) with hot reload.

## Build

```
npm run build
```

Outputs the production build to `dist/`. Preview it locally with:

```
npm run preview
```

## Deployment

GitHub + Cloudflare Pages:

1. Push this repo to GitHub.
2. In Cloudflare Pages, create a project connected to the repo.
3. Settings:
   - Framework preset: `Vite`
   - Build command: `npm run build`
   - Build output directory: `dist`
   - Root directory: `/`
4. Every push to `main` redeploys automatically.

## Structure

```
index.html          single-page markup + inline styles
public/assets/       logo + product screenshots (served as-is, unhashed)
```
