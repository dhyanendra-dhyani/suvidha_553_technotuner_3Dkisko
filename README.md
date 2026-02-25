# ⬡ My 3D Model Showcase

A personal 3D model portfolio site built with Three.js — hosted on Vercel.

## 📁 Project Structure

```
your-project/
├── index.html      ← Main viewer (all-in-one)
├── vercel.json     ← Vercel config for .glb MIME type
├── model.glb       ← YOUR GLB file goes here
└── README.md
```

## 🚀 Deploy to Vercel

1. **Rename your GLB file** to `model.glb` and place it in the root folder
   - OR edit `MODEL_PATH` in `index.html` to match your filename
   - Example: `const MODEL_PATH = './mycar.glb';`

2. **Optionally** change the display name:
   - `const MODEL_DISPLAY_NAME = 'My Awesome Model';`

3. **Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial deploy"
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```

4. **Connect to Vercel:**
   - Go to https://vercel.com → New Project
   - Import your GitHub repo
   - Framework: **Other** (static)
   - Click Deploy ✅

## 🎮 Controls

| Action | How |
|---|---|
| Rotate | Left mouse drag |
| Pan | Right mouse drag |
| Zoom | Scroll wheel |
| Reset View | R key |
| Auto Rotate | Space |
| Wireframe | W key |
| Screenshot | S key |
| Front/Top/Side/Iso | 1 / 2 / 3 / 4 |
| Toggle Grid | G key |

## ⚠️ Common Issues

- **Model not loading?** → Make sure `.glb` file is in the same folder and `MODEL_PATH` matches
- **404 on Vercel?** → `vercel.json` handles MIME types — make sure it's in root
- **File too large for GitHub?** → Use [Git LFS](https://git-lfs.com) for files > 100MB
