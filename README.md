# Jordan Ross — Producer site

Static one-page case studies for SWAGFLIP, True Dirt, and Freeride MTB.
Works on **Netlify**, **Cloudflare Pages**, or **GitHub Pages** — no build step.

## 1) Add screenshots

See `images/README.md`. Put files in:

- `images/swagflip/`
- `images/truedirt/`
- `images/freeride/`

Then swap the gray placeholders in `index.html` for `<img>` tags (examples in that README). Freeride also has an in-engine `gameplay.mp4` clip on the case study.

## 2) Preview locally

Open `index.html` in a browser, or from this folder:

```bash
npx --yes serve .
```

## 3) Deploy

### Netlify (drag & drop)
1. Zip this folder **or** connect a Git repo.
2. [app.netlify.com/drop](https://app.netlify.com/drop) → drop the folder.
3. Copy the `*.netlify.app` URL into 2K / NLG applications.

### Cloudflare Pages
1. Push this folder to a GitHub/GitLab repo (or use direct upload).
2. Cloudflare Dashboard → Workers & Pages → Create → Pages.
3. Framework preset: **None**. Build command: empty. Output directory: `/` (project root).

### GitHub Pages
1. Push to a repo.
2. Settings → Pages → Deploy from branch → `/` (root).
3. Site URL will be `https://<user>.github.io/<repo>/`.

## Optional
- Add LinkedIn in the contact section (commented placeholder in `index.html`).
- Custom domain later in Netlify/Cloudflare DNS settings.
