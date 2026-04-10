# Intoriee - Interior Service Framer Template 

> **Source:** https://intoriee.framer.website/

---

## 📁 What's Inside

```
📁 your-site/
├── index.html              ← Homepage
├── styles.css              ← All CSS (keep at root level)
├── about/
│   └── index.html          ← /about page (multi-page sites)
├── work/
│   └── index.html          ← /work page (multi-page sites)
├── assets/
│   ├── js/                 ← Framer runtime + all JS chunks
│   ├── images/             ← All images (webp, jpg, png, svg…)
│   ├── fonts/              ← All fonts (woff2, woff…)
│   ├── videos/             ← All videos (mp4, webm…)
│   ├── cursors/            ← Custom cursor assets
│   └── cms/                ← CMS data (offline support)
└── README.md
```

⚡ **100% self-contained** — All assets are local files. No Framer subscription or internet needed once hosted.

---

## 🖥️ Run Locally (Preview on your computer)

> ⚠️ **Do NOT open index.html by double-clicking it.**
> Browsers block JavaScript modules on `file://` — you need a local server.

### Step 1 — Install Node.js (skip if you already have it)

Download from **https://nodejs.org** → choose the **LTS version** → install it.

To check if it's already installed, open Terminal and run:
```bash
node -v
```
If you see something like `v20.x.x` → you're good to go. ✅

### Step 2 — Open Terminal in this folder

**Mac:** Right-click the folder in Finder → **"New Terminal at Folder"**
**Windows:** Shift + Right-click the folder → **"Open PowerShell window here"**

### Step 3 — Start the local server

```bash
npx serve .
```

First time? It may ask:
> *"Need to install the following packages: serve — Ok to proceed? (y)"*

Type **y** and press **Enter**.

### Step 4 — Open your browser

Go to → **http://localhost:3000** 🎉

Your site is now running locally! All pages, animations, fonts, and videos will work exactly as expected.

### Option 4 — GitHub Pages (Great for portfolios)

1. Create a new repo at **https://github.com/new**
2. Upload all files from this folder to the repo root
3. Go to repo **Settings → Pages**
4. Source: **Deploy from branch** → main → / (root)
5. Save → your site is live at **https://yourusername.github.io/repo-name** ✅

## 🔧 Troubleshooting

| Problem | Fix |
|---|---|
| **Blank page** | Use `npx serve .` — don't open index.html directly |
| **Images missing** | Re-extract on a faster connection (large sites may timeout) |
| **Sub-pages 404 locally** | Make sure you're in the right folder when running `npx serve .` |
| **Fonts look different** | Check browser settings — fonts are embedded locally and should match |
| **Netlify sub-pages 404** | Each page is a real file (e.g. `/work/index.html`) — no redirects config needed |
| **Slow to load locally** | Normal for large sites — all assets are local, just large files loading |

