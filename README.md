# laiscarneiro.github.io

Source for [www.laiscarneiro.com](https://www.laiscarneiro.com) — a Jekyll site
built and served by GitHub Pages.

## Editing the site

| What you want to change | File to edit |
| --- | --- |
| Add or update a publication | `_data/publications.yml` |
| Home page text | `index.md` |
| Research page | `research.md` |
| CV page | `cv.md` |
| Menu items, site title, social links | `_config.yml` |
| Colours, fonts, spacing | `assets/css/style.scss` |
| Page shell (header, footer, `<head>`) | `_layouts/default.html` |

Commit to `main` and GitHub Pages rebuilds automatically, usually within a minute.

## Adding a publication

Copy an existing block in `_data/publications.yml` and edit it. Keep your own name
written as `Carneiro, L.` — it is bolded automatically. Set `lead: true` for
first-author papers. The list sorts and groups itself by `year`.

## Colours

The palette is defined once as CSS custom properties at the top of
`assets/css/style.scss`, including a dark-mode block. Change `--plum` to
re-skin the whole site.
