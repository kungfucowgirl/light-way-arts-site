# Light Way Arts Foundation Website

A simple, mobile-responsive one-page site for Light Way Arts Foundation. Built with plain HTML, CSS, and a small amount of JavaScript — no build step required.

## Project structure

```
light-way-arts-site/
├── index.html          # Main page (all sections)
├── css/
│   └── styles.css      # Styles and brand colors
├── js/
│   └── main.js         # Mobile menu and footer year
├── content/            # Approved copy and direction (source of truth)
├── AGENTS.md           # Guidelines for contributors and AI assistants
└── README.md           # This file
```

## Preview locally

You need a local web server so links and fonts load correctly. **Do not** rely on double-clicking `index.html` alone.

### Option A — Python (recommended, usually pre-installed on Mac)

From the project folder:

```bash
cd "/Users/genehwang/Documents/00. G&J Hwang Family/Light Way Arts Foundation/light-way-arts-site"
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.

Press `Ctrl+C` in the terminal to stop the server.

### Option B — Node.js (`npx serve`)

If you have Node.js installed:

```bash
npx serve .
```

Follow the URL printed in the terminal (often port 3000 or 5000).

## Deploy to Netlify

1. Push this folder to a GitHub repository (if you have not already).
2. Sign in at [netlify.com](https://www.netlify.com).
3. **Add new site** → **Import an existing project** → connect your repo.
4. Build settings:
   - **Build command:** leave empty
   - **Publish directory:** `.` (the project root, where `index.html` lives)
5. Deploy. Netlify will give you a `*.netlify.app` URL.

**Drag-and-drop alternative:** In the Netlify dashboard, drag the project folder onto the deploy zone. No Git required.

## Deploy to Vercel

1. Push the project to GitHub.
2. Sign in at [vercel.com](https://vercel.com).
3. **Add New** → **Project** → import your repo.
4. Framework preset: **Other** (static site).
5. Root directory: `.` — no build command needed.
6. Deploy.

Vercel will serve `index.html` from the root automatically.

## Updating content

Edit copy in `index.html` to match approved text in the `/content` folder. Do not add unconfirmed legal, tax, donation, sponsor, grant, or event details without updating `/content` first.

## License

Content © Light Way Arts Foundation. Site code may be used for foundation purposes.
