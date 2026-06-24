# Deployment Guide: GitHub & Vercel
## Polsinello Insights (Ontario)

This guide provides the technical steps required to move the **Polsinello Insights** designs into a live production environment on Vercel via GitHub.

### 1. Repository Setup (GitHub)
To maintain an institutional-grade codebase, follow this structure:

1.  **Create a New Repository:** Initialize a private repository on [GitHub](https://github.com/new) named `polsinello-insights`.
2.  **Local Initialization:**
    ```bash
    git init
    git remote add origin https://github.com/YOUR_USERNAME/polsinello-insights.git
    ```
3.  **Project Architecture:**
    *   `/components`: Exported UI elements (Nav, Sidebar, Gold CTA blocks).
    *   `/pages`: Regional Hubs (Toronto, York, Peel, etc.) and Analytics Dashboards.
    *   `/lib/repliers`: API orchestration for the PropTx™ data feed.
    *   `/public/assets`: Brand logos and the 2026 trajectory shaders.

### 2. Secure API Configuration
**CRITICAL:** Never commit your `REPLIERS_API_KEY` to GitHub.

1.  **Create `.env.local`** in your root directory:
    ```text
    REPLIERS_API_KEY=your_actual_key_here
    FUB_API_KEY=your_fub_key_here
    NEXT_PUBLIC_SITE_URL=https://your-domain.vercel.app
    ```
2.  **Update `.gitignore`**: Ensure it contains `.env*` to prevent accidental leaks.

### 3. Vercel Deployment
Vercel is the recommended host as it handles the **Next.js** serverless functions needed for your AI Appraisal Engine and Repliers data sync.

1.  **Import Project:** Connect your GitHub account to [Vercel](https://vercel.com/new).
2.  **Environment Variables:** During the import step, copy the keys from your `.env.local` into the **Environment Variables** section in the Vercel dashboard.
3.  **Deploy:** Click "Deploy." Vercel will provide a staging URL (e.g., `polsinello-insights.vercel.app`).

### 4. Domain & SSL
1.  **Custom Domain:** Map your official domain (e.g., `insights.polsinello.ca`) in **Vercel Settings > Domains**.
2.  **Canada Central:** Ensure your region is set to **Canada (Central) - Toronto** to maintain data residency compliance for TRREB data.

---
*© 2026 Polsinello Insights | Institutional Deployment Suite*