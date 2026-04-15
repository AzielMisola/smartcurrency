# SmartCurrency — Setup Guide (FREE, Google Gemini version)

AI-powered Philippine peso bill recognition for visually impaired users.
**No credit card required. 100% free.**

## Files
- `index.html` — the web app
- `netlify.toml` — Netlify config
- `netlify/functions/recognize.js` — AI recognition (uses Google Gemini free)
- `README.md` — this file

---

## Setup in 6 steps (~10 minutes)

### Step 1 — Get your FREE Gemini API key
1. Go to **aistudio.google.com**
2. Sign in with your Google account (Gmail works)
3. Click **Get API key** (top right or in the left menu)
4. Click **Create API key** → **Create API key in new project**
5. **COPY THE KEY** that appears
6. Paste it somewhere safe (Notes app)

**✅ No payment, no credit card, no $5 fee. Just free.**

### Step 2 — Upload files to GitHub
1. Go to your repo: **github.com/YOUR-USERNAME/smartcurrency**
2. Click **Add file** → **Upload files**
3. Drag ALL files from this folder into the upload area
4. Type commit message: `Upload SmartCurrency with Gemini`
5. Click **Commit changes**

### Step 3 — Connect to Netlify
1. Go to **app.netlify.com**
2. Sign in with GitHub
3. Click your site (or Add new site → Import from GitHub → pick smartcurrency)
4. Click **Deploy site** if needed
5. Wait ~1 minute

### Step 4 — Add your API key to Netlify (IMPORTANT)
1. In Netlify site → **Site configuration** → **Environment variables**
2. Click **Add a variable** → **Add a single variable**
3. **Key:** `GEMINI_API_KEY`  *(all caps, with underscore)*
4. **Value:** paste your Gemini key from Step 1
5. Click **Create variable**

### Step 5 — Redeploy
1. Click **Deploys** tab
2. Click **Trigger deploy** → **Deploy site**
3. Wait 30 seconds

### Step 6 — Test on your phone
1. Open your Netlify URL on your phone
2. Tap **Start camera** → Allow
3. Hold a peso bill in good lighting
4. Tap **Scan**
5. 🎉

---

## Tips for best accuracy
- **Good lighting** is the most important thing
- **Hold the bill flat**, not folded
- **Fill the dashed box** with the bill
- **Show the front** with the person's face
- If it fails once, tap Scan again — it auto-retries

## Troubleshooting

| Problem | Fix |
|---|---|
| "Server missing GEMINI_API_KEY" | You skipped Step 5. Redeploy. |
| "Gemini API error 400" | Wrong API key. Make a new one and redo Step 4. |
| "No bill detected" | Better lighting, fill the frame |
| Camera won't open | Use Chrome or Safari, allow permission |

## About Gemini Free Tier
Google Gemini 2.0 Flash is free for personal projects with generous limits:
- Free tier: 15 requests per minute, 1,500 requests per day
- More than enough for demos, testing, and daily use
- No credit card needed ever

## Project
Vince Dorell Esmero · BSIT 2-C
University of San Agustin · Iloilo
