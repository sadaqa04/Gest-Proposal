# GEST AI Proposal Generator

A live AI-powered proposal generator for GEST — Water & Wastewater Equipment, Jeddah KSA.

---

## Deploy in 5 minutes (Vercel — free)

### Step 1 — Get your Anthropic API key
1. Go to https://console.anthropic.com
2. Sign in or create a free account
3. Click **API Keys** → **Create Key**
4. Copy the key (starts with `sk-ant-...`)

### Step 2 — Upload to GitHub
1. Go to https://github.com and sign in (or create a free account)
2. Click **New repository** → name it `gest-proposal` → click **Create repository**
3. Click **uploading an existing file**
4. Drag and drop the entire `gest-proposal` folder contents
5. Click **Commit changes**

### Step 3 — Deploy on Vercel
1. Go to https://vercel.com and sign in with your GitHub account
2. Click **Add New → Project**
3. Select your `gest-proposal` repository → click **Import**
4. Click **Environment Variables** and add:
   - Name: `ANTHROPIC_API_KEY`
   - Value: your key from Step 1
5. Click **Deploy**

### Step 4 — Your live URL
Vercel gives you a URL like: `https://gest-proposal.vercel.app`

Open it — the proposal generator is live and working!

---

## Files in this project

```
gest-proposal/
├── public/
│   └── index.html       ← The full proposal generator UI
├── api/
│   └── generate.js      ← Secure backend that calls Anthropic API
├── vercel.json          ← Vercel routing config
├── package.json         ← Project metadata
└── README.md            ← This file
```

---

## How it works

1. User fills in project details on the webpage
2. Browser sends the details to `/api/generate` (your secure backend)
3. The backend calls Anthropic's Claude API using your secret API key
4. Claude generates the proposal and returns it
5. The proposal appears on screen — ready to copy or print as PDF

The API key is **never exposed** to the browser. It stays secure on Vercel's servers.

---

## Support
Built for GEST · info@gest-sa.com · +966 12 2636919
