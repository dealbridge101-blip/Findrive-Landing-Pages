# FinDrive Nigeria — Landing Pages

## Vercel Deployment Instructions

### Step 1 — Add the logo
Place your `FinDrive_Logo.png` file in this folder (same level as `index.html`).

### Step 2 — Deploy to Vercel

**Option A — Drag and drop (fastest)**
1. Go to [vercel.com](https://vercel.com) and sign up/log in
2. Click **"Add New Project"** → **"Browse"**
3. Drag this entire folder into the upload area
4. Click Deploy — done in 60 seconds

**Option B — GitHub (recommended for updates)**
1. Push this folder to a GitHub repo
2. Connect the repo to Vercel
3. Every future `git push` auto-deploys

### Step 3 — Connect your domain (findrive.ng)
1. In Vercel project → Settings → Domains
2. Add `findrive.ng` and `www.findrive.ng`
3. Update your DNS at your domain registrar:
   - A record: `76.76.21.21`
   - CNAME (www): `cname.vercel-dns.com`

## Pages & URLs

| File | URL on findrive.ng | Purpose |
|------|-------------------|---------|
| `index.html` | `findrive.ng` | Main homepage |
| `car-finance.html` | `findrive.ng/car-finance` | Car finance leads (Google Ads) |
| `insurance.html` | `findrive.ng/insurance` | Insurance leads |
| `fleet.html` | `findrive.ng/fleet` | B2B/corporate fleet |
| `calculator.html` | `findrive.ng/calculator` | Finance calculator (SEO/email) |
| `guide.html` | `findrive.ng/guide` | Free guide lead magnet |

## Tracking
- **Google Analytics:** G-ZX2WN0W064 (already embedded)
- **Meta Pixel:** 1261139099130940 (already embedded)
- All form submits fire `generate_lead` GA4 event + Meta `Lead` pixel event
- WhatsApp button fires `whatsapp_click` GA4 event + Meta `Contact` pixel event

## WhatsApp Number
Update the WhatsApp number in the `openWA()` function in each file:
```
window.open('https://wa.me/2348000000000?text=...')
```
Replace `2348000000000` with your actual FinDrive WhatsApp number.
