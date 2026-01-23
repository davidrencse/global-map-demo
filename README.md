```md
# Global Social Sentiment – Globe + Side Dashboards

Interactive globe visualization that highlights countries with social posts over a selectable time window, with lightweight side dashboards for quick breakdowns.

**Live demo:** https://global-map-demo.vercel.app :contentReference[oaicite:0]{index=0}

---

## What it does

- **Country highlighting:** Countries with posts in the selected month are highlighted (wire borders). :contentReference[oaicite:1]{index=1}  
- **Time window controls:** Set **Start** / **End**, **Apply**, **Reset**, and use **Play** for timeline animation. :contentReference[oaicite:2]{index=2}  
- **Side dashboards:**
  - “Countries with posts”
  - “Posts by platform” :contentReference[oaicite:3]{index=3}

---

## Project structure

- `index.html` – main entry point (static site) :contentReference[oaicite:4]{index=4}  
- `assets/` – static assets :contentReference[oaicite:5]{index=5}  
- `data/` – data files consumed by the visualization :contentReference[oaicite:6]{index=6}  
- `requirements.txt` – Python dependencies (likely used for data preparation / preprocessing) :contentReference[oaicite:7]{index=7}  

---

## Run locally

Because the repository is **HTML-only** at the top level, you can typically run it as a static site:

### Option A: Simple local server (recommended)
From the repo root, run any static server (examples):

- Python:
  - `python -m http.server 8000`
- Node:
  - `npx serve .`

Then open `http://localhost:8000` and load `index.html`.

### Option B: Open directly
You can often open `index.html` directly in a browser, but some browsers block `fetch()`/module loading from `file://` URLs. If anything fails to load, use Option A.

---

## Notes on data

The UI indicates the app aggregates:
- which **countries** have posts in the selected period, and
- distribution of posts by **platform**. :contentReference[oaicite:8]{index=8}  

Data inputs are expected under `data/`. :contentReference[oaicite:9]{index=9}

---

## Deployment

A live deployment is available on Vercel: https://global-map-demo.vercel.app :contentReference[oaicite:10]{index=10}

---

## Author

By David Ren (david.ren@nyu.edu). :contentReference[oaicite:11]{index=11}

---

## License

No license file is visible from the repository listing. If you intend others to reuse this, add a `LICENSE` (MIT/Apache-2.0 are common choices). :contentReference[oaicite:12]{index=12}
```
