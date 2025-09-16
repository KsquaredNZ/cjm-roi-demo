
# CJM ROI Calculator (React + Vite + Tailwind)

A lightweight, dependency-free web app you can deploy to **Vercel** or **Netlify**.
It includes a **Simple (3 levers)** mode and an **Expanded (10 behaviours → 4 levers)** mode.

## 1) Local run (optional)
```bash
npm install
npm run dev
```
Open the URL shown in the terminal (e.g. http://localhost:5173).

## 2) Deploy to Vercel (step-by-step)
1. Create a new GitHub repo (e.g. `cjm-roi-demo`) and upload these files.
2. Go to https://vercel.com → **New Project** → select your repo.
3. Framework Preset: **Vite** (auto-detected). If not, set it manually.
4. Build settings (defaults):
   - Build Command: `npm run build`
   - Output Directory: `dist`
5. Click **Deploy**. When finished, you’ll get a URL like `https://cjm-roi-demo.vercel.app`.

### Tips
- No env vars needed. If you ever see a 404 after deploy, go to **Settings → Build & Development Settings** and confirm the output directory is `dist`.

## 3) Deploy to Netlify
1. Push the project to GitHub.
2. In https://app.netlify.com → **Add new site** → **Import an existing project**.
3. Select the repo. Build Command: `npm run build`. Publish directory: `dist`.
4. Click **Deploy site**. You’ll get a URL like `https://cjm-roi-demo.netlify.app`.

## 4) Customise branding
- Update `<title>` in `index.html`.
- Add a logo in `App.jsx`, or a favicon in `index.html`.

## 5) Demo flow
- Start in **Simple** mode for speed. Flip to **Expanded** to show the 10 behaviours driving ROI across Conversion, Retention, Cycle-time, and People.
- Tune coefficients to match a client’s pilot benchmarks on the fly.
