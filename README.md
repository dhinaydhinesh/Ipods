# 🎵 iPod Classic Store — Setup Guide

## 📁 Folder Structure

```
ipod-store/
│
├── index.html        ← Main website file (edit this)
├── images/           ← Put ALL your product images here
│   ├── hero.jpg
│   ├── ipod5g-front.jpg
│   ├── ipod5g-back.jpg
│   └── ...
│
└── videos/           ← Put ALL your product videos here
    ├── ipod5g-demo.mp4
    ├── ipod6g-demo.mp4
    └── ...
```

---

## ✏️ How to Edit the Website

Open `index.html` in any text editor (Notepad, VS Code, etc.)
Search for the text "CHANGE THIS" — every place you need to edit is marked.

### Things to change:

| What | Where in the file | Example |
|------|-------------------|---------|
| Store name | Near top & footer | `YOUR Store Name` → `Dhinay's iPod Classics` |
| WhatsApp number | `WHATSAPP_NUMBER` variable | `"91XXXXXXXXXX"` → `"919876543210"` |
| Accent color | `:root { --accent: }` | `#D45F2E` → any hex color |
| Logo image | Inside `<nav>` comments | Uncomment the `<img>` tag |
| Hero image | Inside `.hero-visual` | Uncomment the `<img>` tag |
| Product prices | In the `products` array | `"₹4,500"` |
| Product specs | In each product's `specs:` | Add/remove rows |
| Product images | In each product's `images:` | `["images/front.jpg", "images/back.jpg"]` |
| Product video | In each product's `video:` | `"videos/demo.mp4"` |
| Mark as sold | In each product's `sold:` | `false` → `true` |

### Adding a new iPod:
In `index.html`, find `// ── ADD MORE iPODS` and copy-paste a product block above it.

---

## 🌐 How to Put It Live on GitHub Pages (Free Hosting)

### Step 1 — Create a GitHub account
Go to https://github.com and sign up (free).

### Step 2 — Create a new repository
1. Click the **+** button (top right) → **New repository**
2. Name it: `ipod-store` (or anything you like)
3. Set to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
1. On your new repo page, click **"uploading an existing file"**
2. Drag and drop your entire `ipod-store` folder contents:
   - `index.html`
   - `images/` folder (with all photos)
   - `videos/` folder (with all videos)
3. Scroll down → click **Commit changes**

### Step 4 — Enable GitHub Pages
1. Go to your repo → **Settings** (top menu)
2. Scroll to **Pages** (left sidebar)
3. Under **Source**, select **Deploy from a branch**
4. Branch: **main** | Folder: **/ (root)**
5. Click **Save**

### Step 5 — Your website is live! 🎉
Wait 1–2 minutes, then visit:
```
https://YOUR-GITHUB-USERNAME.github.io/ipod-store/
```
Example: `https://dhinay.github.io/ipod-store/`

---

## 📸 Tips for Images & Videos

- **Image format**: JPG or PNG, ideally under 500 KB each for fast loading
- **Image size**: 800×800 px minimum for good quality
- **Video format**: MP4 (H.264) works on all phones and computers
- **Video size**: Keep under 50 MB per video for fast loading
- To compress videos for free: use https://www.freeconvert.com/video-compressor

---

## 🔄 Updating the Website Later

Whenever you want to change a price, add a new iPod, or mark one as sold:
1. Edit `index.html` on your computer
2. Go to your GitHub repo
3. Click `index.html` → click the **pencil ✏️ icon** to edit online
   OR upload the new file to replace the old one
4. Changes go live in ~30 seconds

---

## ❓ Common Questions

**Q: Can I use this without GitHub?**
A: Yes! Just open `index.html` directly in your browser to preview it locally.

**Q: My images are not showing.**
A: Make sure the file name in the code matches exactly — including uppercase/lowercase. e.g. `ipod.jpg` ≠ `iPod.JPG`

**Q: Can I use a custom domain like `www.dhinayipods.com`?**
A: Yes! Buy a domain from GoDaddy or Namecheap, then in GitHub Pages settings add it under "Custom domain". GitHub has a free guide for this.

**Q: Videos are too large to upload to GitHub?**
A: GitHub has a 100 MB file limit. For large videos, upload to Google Drive, make them public, and embed using an iframe instead.
