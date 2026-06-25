# GitHub Repository Manifest: Polsinello Insights (REVISED)

To resolve the Vercel 404 error, ensure your repository includes the **app/page.tsx** file at the root of your application. This file is what renders your homepage.

## 1. Corrected Directory Structure

```text
/polsinello-insights
├── /app
│   ├── page.tsx                # MISSING FILE: Home Page ({{DATA:SCREEN:SCREEN_41}})
│   ├── layout.tsx              # Root Layout (Nav & Footer)
│   ├── /api
│   │   └── /listings/route.ts  # Repliers API Proxy
│   ├── /hubs                   # Regional Hubs & Town spokes
│   ├── /property/[id]          # Dynamic listing views
│   └── /evaluation             # Home Evaluation tool
├── /components                 # UI Library from Stitch
├── /public
│   └── /assets                 # Logos and Shaders
├── /lib                        # API & AI Logic
├── .env.local                  # API Keys (DO NOT PUSH TO GITHUB)
├── .gitignore                  # Hide .env files
└── package.json                # Dependencies
```

## 2. Troubleshooting the 404
1.  **Check app/page.tsx:** Ensure you have created this file. Without it, your main domain will always return a 404.
2.  **Vercel Build Logs:** Log in to your Vercel Dashboard and check the "Deployments" tab. If the status is "Ready," but you see a 404, it is a routing issue (missing file).
3.  **Framework Preset:** In Vercel Project Settings, ensure the "Framework Preset" is set to **Next.js**.
4.  **Root Directory:** Ensure Vercel is looking at the correct root directory if your code is inside a subfolder in your repo.

---
*© 2026 Polsinello Insights | Technical Support*