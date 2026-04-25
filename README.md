# PGHELPDESK

Prendiville Group Help Desk — FAQs, Preferred Suppliers and Resources.

## Deploy to Vercel (Step-by-step)

### Option A — Drag & Drop (Easiest, no GitHub needed)

1. Install dependencies and build the project locally:
   ```
   npm install
   npm run build
   ```
2. Go to [vercel.com](https://vercel.com) and sign up / log in
3. Click **"Add New Project"**
4. Drag and drop the **`dist`** folder that was created in step 1
5. Click **Deploy** — your site will be live in ~30 seconds

### Option B — GitHub (Recommended for ongoing updates)

1. Create a free account at [github.com](https://github.com)
2. Create a new repository called `pghelpdesk`
3. Upload all these project files to the repository
4. Go to [vercel.com](https://vercel.com) → **Add New Project** → Import from GitHub
5. Select the `pghelpdesk` repository
6. Vercel auto-detects Vite — just click **Deploy**
7. Every time you push changes to GitHub, Vercel redeploys automatically

### Connecting your Crazy Domains domain

1. In Vercel, go to your project → **Settings → Domains**
2. Type in your domain name (e.g. `pghelpdesk.com.au`) and click **Add**
3. Vercel will show you two DNS records, e.g.:
   - **A record**: `@` → `76.76.21.21`
   - **CNAME**: `www` → `cname.vercel-dns.com`
4. Log into **Crazy Domains** → My Domains → Manage → DNS Settings
5. Add those two records exactly as shown
6. Wait 10–30 minutes — your site will be live on your domain!

## Local Development

```bash
npm install      # Install dependencies (first time only)
npm run dev      # Start local dev server at http://localhost:5173
npm run build    # Build for production (creates /dist folder)
```

## Admin Login

Password: `admin123`

Change this in `src/App.jsx` — search for `admin123` and replace with your own password.
