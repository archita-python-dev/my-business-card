# My Business Card

A personal business card built with React

## Tech Stack

| Domain | Technology |
|---|---|
| UI | React 19 (`react`, `react-dom`) |
| Build tool | Vite 8 with `@vitejs/plugin-react` |
| Language | JavaScript (JSX, ES modules) |
| Styling | Plain CSS (`src/index.css`, `src/App.css`) |
| Linting | [oxlint](https://oxc.rs/docs/guide/usage/linter) with the React plugin |

## Getting Started

Requires [Node.js](https://nodejs.org/) 20.19+ or 22.12+ (required by Vite 8) and npm

```bash
git clone https://github.com/archita-python-dev/my-business-card.git
cd my-business-card
npm install
npm run dev
```

Vite prints a local URL (usually <http://localhost:5173>) — open it in your browser
The page hot-reloads as you edit files

## Available scripts

| Command | What it does |
|---|---|
| `npm run dev` | Start the Vite dev server with hot module replacement |
| `npm run build` | Produce a production build in `dist/` |
| `npm run preview` | Serve the built `dist/` locally to check the production output |
| `npm run lint` | Run oxlint over the project |

## Deployment

`npm run build` emits a static site into `dist/`, deployable to GitHub Pages, Netlify,
Vercel, or Cloudflare Pages

Deploying to GitHub Pages under a repo subpath requires setting the base in `vite.config.js`,
otherwise the built page loads blank:

```js
export default defineConfig({
  plugins: [react()],
  base: '/my-business-card/',
})
```