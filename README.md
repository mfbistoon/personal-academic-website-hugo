# Mohsen Farhadloo: Academic Website

Built with the [HugoBlox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv) template,
themed in Concordia University colours (burgundy `#912338`, gold `#cbb576`).

## Run locally

```bash
pnpm install
hugo server        # http://localhost:1313
```

Build for production: `hugo --gc --minify` (output in `public/`).

## Where to edit

| What | File |
| --- | --- |
| Name, bio, education, links, interests | `data/authors/me.yaml` |
| Profile photo | `assets/media/authors/me.jpg` |
| Homepage sections | `content/_index.md` |
| Publications (one folder each: `index.md` + `cite.bib`) | `content/publications/` |
| Research projects | `content/projects/` |
| News items | `content/news/` |
| Teaching | `content/teaching.md` |
| CV PDF (menu "CV" + "Download CV" button) | `static/uploads/cv.pdf` |
| Menu | `config/_default/menus.yaml` |
| Colours, site name, header/footer | `config/_default/params.yaml` |
| Site URL (set before deploying) | `config/_default/hugo.yaml` → `baseURL` |

All publications, projects, news, courses and the CV PDF are **sample placeholders**; replace them with your own.

Note: `config/_default/hugo.yaml` explicitly allows the `tailwindcss` CLI under `security.exec.allow`;
Hugo ≥ 0.163 blocks it otherwise and the build fails.
