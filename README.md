# ButBrooo Fantasy Football League — Website

## Files Included
- `index.html` — Main app (all pages in one file)
- `manifest.json` — PWA manifest (enables "Add to Home Screen")
- `sw.js` — Service Worker (offline support)
- `IMG_4608.jpg` — BB circle logo (place in same folder)
- `BUT_BROO_FINAL_ART.png` — ButBrooo banner logo (place in same folder)

## Free Deployment Options

### Option 1: GitHub Pages (Recommended — 100% Free)
1. Create a free account at github.com
2. Create a new repository called `butbrooo`
3. Upload all files (index.html, manifest.json, sw.js, + your 2 image files)
4. Go to Settings → Pages → Source: "main" branch, "/" root
5. Your site will be live at: `https://yourusername.github.io/butbrooo`

### Option 2: Netlify (Free, easiest drag & drop)
1. Go to netlify.com → sign up free
2. Drag and drop your entire folder onto the Netlify dashboard
3. You get a free URL like `butbrooo.netlify.app`
4. Optional: connect a custom domain

### Option 3: Vercel (Free)
1. Go to vercel.com → sign up free
2. Import from GitHub or drag & drop
3. Free URL like `butbrooo.vercel.app`

## Adding to iPhone Home Screen (Safari or Chrome)
1. Open the deployed URL in Safari or Chrome on your iPhone
2. Tap the Share button (box with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Name it "ButBrooo" and tap Add
5. It will appear as an app icon on your home screen!

## How to Update the Timeline
The timeline saves to your browser's localStorage. To add events:
- Tap the "+ Add Event" button on the Timeline page
- Enter the year and description
- Tap "Add Event"

To make timeline edits permanent (visible to all members):
- Edit the `DEFAULT_TIMELINE` array in index.html
- Re-deploy the file

## How to Update League Members
Find the `MEMBERS` array in index.html (search for `const MEMBERS = [`).
Edit each member's:
- `name` — Display name
- `initials` — 2-letter initials shown in avatar
- `team` — Subtitle shown under name
- `wins`, `losses`, `championships` — Stats (use numbers or "–" for TBD)
- `bio` — Description shown when you tap their profile
- `badge` — "comm" (gold), "loser" (red), null (none)

## Pages
- **Home** — Hero page with quick nav, social links, ticker
- **Timeline** — Scrollable league history with add-event feature
- **Stats** — Embedded Google Sheets + quick stat cards
- **League** — Member profiles with tap-to-expand cards
- **Social** — Twitter/Instagram links, sponsor showcase
