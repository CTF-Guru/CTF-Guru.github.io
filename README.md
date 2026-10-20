# ctf.guru — the main landing page

This repo **is** the ctf.guru site: `CTF-Guru/CTF-Guru.github.io`, the GitHub Pages **org site**.
It holds `CNAME=ctf.guru` + the shared HTTPS cert, and GitHub serves the org's project repos
under it at `ctf.guru/<repo>/` (e.g. `ctf.guru/security`, `ctf.guru/ai`).

- **`index.html`** — the landing page. A single self-contained static file (CSS/JS/images inline).
  Edit it directly here; commit + push and GitHub Pages redeploys.
- **`CNAME`** — `ctf.guru` (only this org-site repo carries it; project repos inherit the domain).
- **`.nojekyll`** — serve files as-is.

The explainer libraries (`ctf.guru/ai`, `ctf.guru/security`) and the News Flash (`ctf.guru/newsflash`) are
separate repos with their own builders; this repo is only the landing page.

## Deploy
```bash
git add -A && git commit -m "…" && git push        # Pages rebuilds automatically
```
