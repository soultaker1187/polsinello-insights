# GitHub Repository Manifest: Polsinello Insights (Final)

To move these high-fidelity designs into a production environment, follow this structured roadmap. This architecture is optimized for **Next.js 14** and **Tailwind CSS**.

## 1. Directory Structure

```text
/polsinello-insights
├── /app
│   ├── /api
│   │   └── /listings/route.ts  # Repliers API Proxy
│   ├── /hubs                   # Regional Hubs & Town spokes
│   ├── /property/[id]          # Dynamic listing views
│   ├── /evaluation             # Home Evaluation tool
│   └── layout.tsx              # Global Nav & Footer with social links
├── /components                 # Exported UI elements
│   ├── /navigation
│   ├── /charts                 # Recharts/Chart.js implementations
│   └── /marketing              # "Since 1989" trust blocks
├── /public
│   └── /assets                 # Logos, Hero Shaders, Property images
├── /lib
│   ├── /repliers               # PropTx™ API Orchestration
│   └── /ai                     # Appraisal Logic Microservice
├── .env.local                  # Secure API Keys (DO NOT PUSH)
├── .gitignore                  # Configured to hide .env
└── package.json                # Dependencies: mapbox-gl, framer-motion, tailwind
```

## 2. Technical Hand-off Steps

### Step 1: Export Code
Use the **"</> View Code"** button in Stitch for each screen to capture the JSX and Tailwind structures. Place these into your `/app` directory corresponding to the hub or tool name.

### Step 2: Configure Environment
Create a `.env.local` file with:
- `REPLIERS_API_KEY`: Your PropTx access key.
- `FUB_API_KEY`: For Follow Up Boss lead sync.
- `MAPBOX_ACCESS_TOKEN`: For the interactive discovery maps.

### Step 3: Deploy to Vercel/AWS
Connect your GitHub repo to **Vercel** for seamless deployment. Ensure the region is set to **Canada (Central)** to comply with TRREB data residency policies.

---
*© 2026 Polsinello Insights | Since 1989*