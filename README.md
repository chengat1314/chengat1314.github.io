# chengat1314.github.io

Personal site for **Cheng Feng**: *Data platform strategy, with cost-efficient infrastructure.*

Plain HTML + CSS, no build step. Light/dark mode follows the system setting.

## Files
- `index.html`: the single page (hero, about, focus areas, writing, recognition, speaking, contact)
- `styles.css`: all styling
- `favicon.svg`: "FC" monogram
- `og.png`: 1200×630 social preview image
- `404.html`, `robots.txt`, `sitemap.xml`, `.nojekyll`

## Publish on GitHub Pages
1. Create a public repo named **`chengat1314.github.io`** under github.com/chengat1314.
2. Push these files to the `main` branch root:
   ```bash
   git init && git add . && git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/chengat1314/chengat1314.github.io.git
   git push -u origin main
   ```
3. Repo **Settings → Pages**: Source = *Deploy from a branch*, Branch = `main` / `(root)`.
4. The site goes live at https://chengat1314.github.io within a minute or two.

## Updating
- **Add a blog post:** copy a `<a class="post card">` block in the *Writing* section.
- **Add a talk:** in the *Speaking* section, uncomment the `<ul class="talks">` template and add one `<li>` per talk.
- **Cost post:** when the cost-efficiency article is out, replace the "Writing soon" tag in Focus area 06 with a link.
- Bump `<lastmod>` in `sitemap.xml` after changes.

Preview locally: `python3 -m http.server` then open http://localhost:8000.
