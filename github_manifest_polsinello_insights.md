# GitHub Repository Manifest: Polsinello Insights

To move from these high-fidelity designs to a live production environment, your developers should structure the GitHub repository as follows. This architecture is optimized for **Next.js** and **Tailwind CSS**, as outlined in your technical specifications.

## 1. Directory Structure

```text
/polsinello-insights
├── /components         # UI elements exported from Stitch (Nav, Sidebar, Gold CTA blocks)
├── /pages              # Regional Hubs and Analytics Dashboards (Toronto, York, etc.)
├── /public
│   └── /assets         # Brand logos, property images, and hero shaders
├── /lib
│   ├── /repliers       # Logic for syncing with the PropTx™ / Repliers API
│   └── /ai             # Appraisal engine logic and weighting variables
├── /styles             # Global CSS and Tailwind configuration
├── .env.local          # LOCAL ONLY: Your API Keys (Never push this to GitHub!)
├── .gitignore          # Configured to ignore .env files
├── package.json        # Project dependencies and scripts
└── README.md           # Project overview and setup instructions
```

## 2. What to Export from Stitch

For each screen in your project, your developers should use the **"</> View Code"** button to capture:

1.  **HTML/JSX Structure:** Place these in the corresponding files within `/pages` or `/components`.
2.  **Tailwind Classes:** Ensure your `tailwind.config.js` is set up to support the Polsinello brand palette (#0f172a Deep Slate and #d4af37 Polsinello Gold).
3.  **Assets:** Download all brand-specific images and logos and place them in `/public/assets`.

## 3. Essential Configuration Files

### .gitignore (Crucial for Security)
Ensure this file exists in your root directory to prevent leaking your Repliers and Follow Up Boss API keys.
```text
# api keys
.env
.env.local

# dependencies
node_modules
.next
```

### package.json
I have already generated a tailored `package.json` ({{DATA:DOCUMENT:DOCUMENT_212}}) containing all the necessary dependencies like `mapbox-gl`, `chart.js`, and `tailwindcss`.

---
*Refer to your **GitHub & Vercel Deployment Guide** ({{DATA:DOCUMENT:DOCUMENT_100}}) for step-by-step terminal commands to initialize the repo.*