# GEST AI Demo Portal

All 4 AI demos in one website — built for the Thursday meeting.

## Deploy to Vercel (10 minutes, free)

### 1. Get your Anthropic API key
- Go to https://console.anthropic.com → API Keys → Create Key
- Copy the key (starts with `sk-ant-...`)

### 2. Push to GitHub
- Go to https://github.com → New repository → name: `gest-ai-demo`
- Upload all files from this folder
- Commit

### 3. Deploy on Vercel
- Go to https://vercel.com → sign in with GitHub
- Add New → Project → Import `gest-ai-demo`
- Under **Environment Variables**, add:
  - `ANTHROPIC_API_KEY` = your key from step 1
- Click **Deploy**

### 4. Your URL is live
You get a URL like `gest-ai-demo.vercel.app` — open it on your laptop for the meeting.

## What's inside

- **Overview tab** — intro to all 4 systems + full company AI roadmap
- **Proposal Generator** — fill in project details, get a full proposal in 15 seconds
- **Project Dashboard** — all GEST projects, click for details, ask AI questions
- **Technical Support Chat** — Arabic/English chatbot for equipment questions
- **Tender Analyzer** — paste any tender, AI scores GEST's fit and flags risks

## Files

```
gest-demo-portal/
├── index.html        ← Full portal (all 4 demos in one page)
├── api/
│   └── generate.js   ← Secure API route (keeps your key safe)
├── vercel.json       ← Routing config
├── package.json
└── README.md
```
