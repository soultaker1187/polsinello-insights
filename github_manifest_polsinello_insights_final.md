# GitHub Repository Manifest: Polsinello Insights (Final)

To move from these high-fidelity designs to a live production environment, your developers should structure the GitHub repository as follows. This architecture is optimized for **Next.js 14 (App Router)** and **Tailwind CSS**.

## 1. Directory Structure

```text
/polsinello-insights
├── /app
│   ├── /api
│   │   └── /listings/route.ts  # Repliers API Proxy
│   ├── /hubs
│   │   ├── /toronto/page.tsx   # {{DATA:SCREEN:SCREEN_229}}
│   │   ├── /york/page.tsx      # {{DATA:SCREEN:SCREEN_120}}
│   │   ├── /peel/page.tsx      # {{DATA:SCREEN:SCREEN_213}}
│   │   ├── /hamilton/page.tsx  # {{DATA:SCREEN:SCREEN_136}}
│   │   ├── /ottawa/page.tsx    # {{DATA:SCREEN:SCREEN_134}}
│   │   ├── /niagara/page.tsx   # {{DATA:SCREEN:SCREEN_23}}
│   │   └── ... (All 20+ Hubs)
│   ├── /property/[id]/page.tsx # {{DATA:SCREEN:SCREEN_170}}
│   ├── /valuation/page.tsx     # {{DATA:SCREEN:SCREEN_151}}
│   └── layout.tsx              # Root Layout with Nav & Footer
├── /components                 # Shared UI elements exported from Stitch
│   ├── /navigation
│   ├── /charts
│   └── /marketing
├── /public
│   └── /assets                 # Brand logos, property images, and hero shaders
├── /lib
│   ├── /repliers               # PropTx™ / Repliers API Orchestration
│   └── /ai                     # The Data Architect Appraisal Logic
├── /styles                     # Tailwind configuration and globals
├── .env.local                  # API Keys (Never push to GitHub)
├── package.json                # {{DATA:DOCUMENT:DOCUMENT_226}}
└── README.md                   # {{DATA:DOCUMENT:DOCUMENT_98}}
```

## 2. Technical Synchronization
*   **Data Residency:** All production instances must be deployed to **AWS Canada (Central)** to comply with TRREB data policies.
*   **Live Sync:** Use React Query or SWR to handle the sub-second polling for "Live Market Feed" indicators.
*   **AEO/SEO:** Ensure the JSON-LD schemas defined in the Technical SEO Audit are injected into every hub and property page.

## 3. Communication Integration
Ensure the frictionless **(905) 830-9111** call/text triggers are configured as primary CTAs across the mobile and desktop views to maintain high lead conversion.

---
*© 2026 Polsinello Insights | Since 1989*