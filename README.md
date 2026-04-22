# Contractor Verified — Austin App

Mobile-first React app for Austin's vetted contractor network. Connects homeowners and realtors with 246+ verified construction, tile, flooring, and home-service professionals.

---

## 🚀 Deploy in 5 minutes (GitHub → Vercel)

### Step 1: Create a GitHub repo (1 minute)
1. Go to **https://github.com/new**
2. Name it `cv-app` (or anything you like)
3. Keep it **Private** if you want (Vercel works either way)
4. Click **Create repository**
5. On the next page, click the link **"uploading an existing file"**

### Step 2: Upload this project (1 minute)
1. Unzip the file you downloaded
2. Open the unzipped `cv-app` folder
3. **Select all files and folders inside** (use Cmd+A on Mac). Important: select the *contents*, not the outer folder.
4. Drag them onto the GitHub upload page
5. Scroll down and click **Commit changes**

### Step 3: Deploy on Vercel (2 minutes)
1. Go to **https://vercel.com/signup**
2. Click **Continue with GitHub** (free, no credit card)
3. Once logged in, click **Add New → Project**
4. Find `cv-app` in your repo list and click **Import**
5. Don't change anything on the config screen — Vercel auto-detects Vite
6. Click **Deploy**

~60 seconds later you'll see 🎉 and a live URL like `cv-app-abc123.vercel.app`.

### Step 4 (optional): Custom domain
In your Vercel project → **Settings → Domains**, add `app.contractorverifiedatx.com`. Then in your domain DNS (Wix), add the CNAME record Vercel gives you. Done.

---

## 🔑 Demo login

- **Admin** (you): `admin@contractorverified.com` / `admin123`
- **Other roles** (Homeowner / Contractor / Realtor): pick role on welcome screen → click "Create account" → use any email/password

---

## 🛠 Local development (optional)

Requires Node.js 18+.

```bash
npm install
npm run dev          # start dev server at http://localhost:5173
npm run build        # production build → dist/
npm run preview      # preview built version
```

---

## 📝 Notes

- **Storage:** The deployed app uses `localStorage` (per-browser). Each visitor has their own data. Perfect for demos. If you later want shared/global data across users, we'd need a real backend (Supabase, Firebase, etc.).
- **Seed data:** 246 contractors auto-load for every visitor (from `SEED_MEMBERS` in `src/App.jsx`).
- **Updates:** Push changes to GitHub → Vercel auto-redeploys in ~60 seconds.
