# M Marcelo Arief — Portfolio

A static, dependency-free portfolio site. No build step, no framework — just three files.

## Structure

```
.
├── index.html      # markup + content
├── css/
│   └── styles.css  # all styling (design tokens at the top)
└── js/
    └── script.js   # mobile nav toggle, scroll-spy nav highlight, back-to-top button
```

## Before you publish

Open `index.html` and replace the two placeholder links (search for `href="#"`):
- LinkedIn URL
- Portfolio URL (if you have one hosted elsewhere)

## Running locally

Just open `index.html` in a browser — everything is relative paths and CDN fonts,
no server required. (Some browsers restrict `fetch`/module scripts under `file://`,
but this project doesn't use any, so it works fine.)

## Deploying to GitHub Pages

1. Create a new GitHub repository (public).
2. Upload all files, **keeping the folder structure** (`css/styles.css` and `js/script.js`
   must stay in their subfolders — GitHub's drag-and-drop upload preserves folders if you
   drag the whole `css` and `js` folders in, not just the files inside them).
3. Go to **Settings → Pages**, set Source to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. Save, wait ~1–2 minutes, then visit the URL GitHub shows you.

## Editing content later

- Text/content changes → `index.html`
- Colors, spacing, fonts → `css/styles.css` (see the `:root` variables at the top)
- Behavior (mobile menu, scroll highlighting, back-to-top button) → `js/script.js`
