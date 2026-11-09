# Syed Rizwan Uddin · Portfolio

Plain HTML, CSS and JavaScript. No build step, no framework, no dependencies.

```
index.html   the whole site (styles + scripts inline)
resume.pdf   linked from the "Resume" buttons
```

## Preview locally

```bash
cd portfolio
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy on Vercel (free Hobby plan)

1. Create a **public** GitHub repo called `portfolio`.
2. Upload `index.html`, `resume.pdf` and this README (GitHub web: **Add file → Upload files → Commit**).
3. Go to vercel.com and sign up **with GitHub** (Hobby plan, free).
4. **Add New → Project →** import `portfolio`.
   - Framework Preset: **Other**
   - Build command: leave empty
   - Output directory: leave empty (root)
5. Click **Deploy**. You get a URL like `portfolio-xxxx.vercel.app`.
6. **Settings → Domains →** edit it to something clean, e.g. `syedrizwanuddin.vercel.app` (if free).
7. Every `git push` to `main` redeploys automatically.

Share the **production domain** from step 6. Preview URLs (the long ones with random
hashes) can sit behind Vercel login, so recruiters may not be able to open them.

## Or: GitHub Pages (also free)

1. Create a public repo named exactly `rizwanuddin.github.io`.
2. Upload `index.html` and `resume.pdf` to the root.
3. **Settings → Pages →** Source: *Deploy from a branch*, Branch: `main`, Folder: `/ (root)`.
4. Live at `https://rizwanuddin.github.io` in a minute or two.

## Updating

- New resume: replace `resume.pdf` (keep the same name).
- New project: copy one `<article class="case">` block in `index.html` and edit the text.
- Skills "used in" text lives in each button's `data-used` attribute.
