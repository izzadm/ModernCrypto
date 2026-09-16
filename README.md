# Modern Cryptography — exam notes

Static revision site for Modern Cryptography (Korea University, Changmin Lee).

```
crypto-notes/
├── index.html                    hub page, lecture list
├── 01-introduction.html
├── 02-symmetric-encryption.html
├── assets/style.css              shared stylesheet
└── README.md
```

## Publishing on GitHub Pages

1. Create a repository, e.g. `crypto-notes`.
2. Upload the contents of this folder to the repository root, keeping `assets/` as a folder.
3. Repo → **Settings** → **Pages** → Source: *Deploy from a branch*, Branch: `main`, Folder: `/ (root)` → **Save**.
4. The site appears at `https://<username>.github.io/crypto-notes/` within a minute or two.

All links are relative, so it works at a subpath without changes. No build step, no dependencies beyond two Google Fonts (the pages fall back to Georgia and a system monospace if fonts are blocked).

## Adding lecture 3

1. Copy `02-symmetric-encryption.html` to `03-<topic>.html`.
2. Replace the `<title>`, the `<h1>`, the table of contents list, and the article body.
3. Fix the two links in the `.pager` at the bottom, and the "Next lecture" text at the end of lecture 02.
4. Add one `<li>` to the `.deck` list in `index.html` (there is a greyed-out placeholder to replace).

## Conventions

| Element | Meaning |
|---|---|
| `<div class="box def">` | Definition — the statement to memorise |
| `<div class="box ex">` | Worked example |
| `<div class="box attack">` | Attack and its cost |
| `<div class="box tip">` | Exam framing / things that get asked |
| `<div class="formula">` | Monospace block, whitespace preserved |
| `<table class="grid">` | Numeric tables (permutation tables, S-boxes) |
| `<table class="prose">` | Comparison tables read as sentences |

Dark mode follows the OS setting. Every page has a print stylesheet — Ctrl/Cmd+P drops the navigation.
