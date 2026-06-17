# Hachi × Plusone — Emotional Coordinates

Four-page brand object (Presentation · Brand Guidelines · Crossmodal Coffee · BrandBook),
unified under the BrandBook design system. Served at **https://plusone.hachiproject.com**.

---

## Finish publishing — 3 steps

### 1. Upload the site file as `index.html`
The HTML is ~2.2 MB (embedded photography), so it is added manually:
- GitHub web UI: **Add file → Upload files**, drag in the delivered
  `Plusone_Emotional_Coordinates_Unified.html`, **rename it to `index.html`**, commit to `main`.
- Or via git:
  ```bash
  git clone https://github.com/Matheus-Anchora/plusone.git
  cp Plusone_Emotional_Coordinates_Unified.html plusone/index.html
  cd plusone && git add index.html && git commit -m "Add site" && git push
  ```

### 2. Turn on GitHub Pages
**Settings → Pages → Build and deployment**
- Source: **Deploy from a branch**
- Branch: **main** / **/ (root)** → **Save**
- The custom domain `plusone.hachiproject.com` is read from the `CNAME` file in this repo.
- After DNS resolves, tick **Enforce HTTPS**.

### 3. Add the DNS record at GoDaddy (hachiproject.com)
Add a **CNAME** record:

| Type  | Name      | Value (Points to)             | TTL     |
|-------|-----------|-------------------------------|---------|
| CNAME | `plusone` | `matheus-anchora.github.io`   | default |

DNS can take from a few minutes up to ~an hour to propagate. Once it does,
the site is live at https://plusone.hachiproject.com
