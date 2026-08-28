# Jordan Ross — Producer site

Static one-page case studies for SWAGFLIP, True Dirt, and Freeride MTB.
No build step. Live on **Vercel**:

**https://jordan-ross-producer.vercel.app/**

GitHub already lists that URL as the repo homepage. Pushes to `main` create Production deployments (Vercel Git integration).

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

## 3) Deploy (Vercel — already connected)

This repo is already linked. After a push to `main`, Vercel rebuilds Production. Check:

- Live site: [jordan-ross-producer.vercel.app](https://jordan-ross-producer.vercel.app/)
- GitHub Production deployments: [github.com/jordross/jordan-ross-producer/deployments](https://github.com/jordross/jordan-ross-producer/deployments)
- Vercel dashboard: [vercel.com/dashboard](https://vercel.com/dashboard) → project `jordan-ross-producer`

`vercel.json` is already in the repo (`cleanUrls`, rewrite `/` → `/index.html`). Framework: **Other** / static. Build command empty. Output directory: project root.

### If you need to reconnect GitHub → Vercel

1. Open [vercel.com/new](https://vercel.com/new) and sign in with the same GitHub account (`jordross`).
2. Import **jordross/jordan-ross-producer**.
3. Leave build command empty. Output directory `.` (root).
4. Deploy. The `*.vercel.app` URL is what goes on resumes / 2K applications.

### Cursor agents (Vercel MCP)

To let a Cursor Cloud / desktop agent list deployments and inspect the project, authenticate the **Vercel** MCP server in Cursor Desktop (Settings → MCP). Until that is signed in, agents can still edit this repo; they cannot call Vercel APIs.

## Other hosts (optional)

Same static files also work on Netlify, Cloudflare Pages, or GitHub Pages — no build step.

### Netlify (drag & drop)
1. Zip this folder **or** connect a Git repo.
2. [app.netlify.com/drop](https://app.netlify.com/drop) → drop the folder.

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
- Custom domain later in Vercel / Netlify / Cloudflare DNS settings.
