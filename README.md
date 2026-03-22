# EduPath v35 — Deployment & Installation Guide

## 🌐 Live URL
https://abdulwahabbadmus001-creator.github.io/Edupathh

---

## 📦 FILES IN THIS PACKAGE

| File | Purpose |
|------|---------|
| `index.html` | The entire app (2.2MB) |
| `admin.html` | Admin dashboard (separate) |
| `sw.js` | Service Worker v12.0 (offline support) |
| `manifest.json` | PWA manifest (install as app) |
| `icon-192.png` | App icon (small) |
| `icon-512.png` | App icon (large) |
| `icon-192.svg` | App icon SVG |
| `icon-512.svg` | App icon SVG |
| `.nojekyll` | Tells GitHub Pages not to process files |
| `404.html` | Handles page-not-found redirects |
| `netlify.toml` | Netlify config (ignore if using GitHub Pages) |
| `netlify/` | Netlify functions folder (ignore if using GitHub Pages) |

---

## 🚀 HOW TO UPLOAD TO GITHUB (EASY METHOD)

### Option A — GitHub Desktop (Recommended)

1. Download **GitHub Desktop** from https://desktop.github.com
2. Sign in with your GitHub account
3. Click **File → Clone Repository**
4. Find `abdulwahabbadmus001-creator/Edupathh` and clone it
5. Open the cloned folder on your computer
6. **Copy all files from this ZIP** into that folder (replace existing files)
7. Open GitHub Desktop — you will see all changed files listed
8. In the bottom left, type: `EduPath v35 update`
9. Click **Commit to main**
10. Click **Push origin** (top right)
11. ✅ Done — live in about 60 seconds

---

### Option B — GitHub Website (Manual, no software needed)

1. Go to https://github.com/abdulwahabbadmus001-creator/Edupathh
2. For each file you want to update:
   - Click the filename (e.g. `index.html`)
   - Click the **pencil icon ✏️** (Edit this file)
   - Select all the existing text and delete it
   - Paste the new file content
   - Scroll down and click **Commit changes**
3. Repeat for: `index.html`, `sw.js`, `manifest.json`, `admin.html`
4. ✅ Done

> ⚠️ Important: `index.html` is very large (2.2MB). GitHub's web editor
> may struggle with it. Use GitHub Desktop if this is the case.

---

### Option C — Git Command Line

```bash
cd /path/to/your/local/Edupathh
cp /path/to/unzipped/files/* .
git add -A
git commit -m "EduPath v35 update"
git push origin main
```

---

## 📱 HOW TO INSTALL ON YOUR PHONE

### Android (Chrome) — Recommended

1. Open **Google Chrome** on your Android phone
2. Visit: https://abdulwahabbadmus001-creator.github.io/Edupathh
3. Wait for the page to fully load
4. Tap the **three dots menu ⋮** at the top right
5. Tap **"Add to Home screen"** or **"Install app"**
6. Tap **Add / Install**
7. ✅ EduPath icon appears on your home screen!

### iPhone / iPad (Safari)

1. Open **Safari** (must be Safari, not Chrome)
2. Visit: https://abdulwahabbadmus001-creator.github.io/Edupathh
3. Tap the **Share button** 📤 at the bottom
4. Scroll down and tap **"Add to Home Screen"**
5. Tap **Add**
6. ✅ EduPath icon appears on your home screen!

> 💡 Once installed, EduPath works fully offline — no internet needed after first load.

---

## 📲 HOW TO SHARE WITH OTHERS

Send this message on WhatsApp to friends and students:

```
📚 *EduPath — Free Nigerian Exam Prep App*

Practice WAEC, NECO and JAMB past questions for FREE!
✅ 5,300+ questions with explanations
🧠 Smart study review
📝 Mock exams (timed)
📴 Works offline — no data needed!

👇 *Install it now (free, no app store needed):*
https://abdulwahabbadmus001-creator.github.io/Edupathh

*How to install:*
Android: Open in Chrome → tap ⋮ menu → "Add to Home Screen"
iPhone: Open in Safari → tap Share 📤 → "Add to Home Screen"
```

---

## 🔑 ADMIN DASHBOARD

**URL:** https://abdulwahabbadmus001-creator.github.io/Edupathh/admin.html?key=wahab2024

**Passcode:** EDU-ADMIN-7X9K2W

Keep these private. The admin dashboard lets you:
- View all registered users and activity
- See flagged questions
- Monitor usage stats
- Add new questions

---

## 💳 ACTIVATING PAYSTACK (When Ready)

The Paystack payment system is fully built. To go live:

1. Create a free account at https://paystack.com
2. Go to **Settings → API Keys** in your Paystack dashboard
3. Copy your **Live Public Key** (starts with `pk_live_...`)
4. Open `index.html` and find this line (around line 11800):
   ```javascript
   const PAYSTACK_PUBLIC_KEY = 'pk_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx';
   ```
5. Replace the `pk_live_xxx...` with your actual key
6. Save and upload to GitHub

**Plans already configured:**
- Monthly: ₦500
- Term (3 months): ₦1,200
- Yearly: ₦3,500

---

## 🌍 GETTING A CUSTOM DOMAIN (When Ready)

A custom domain (e.g. `edupathapp.com.ng`) makes your app look professional
and makes the link easy to share and remember.

**Step 1:** Buy domain (~₦3,000–5,000/year)
- WhoGoHost: https://whogohost.com
- Qserver: https://qserver.ng

**Step 2:** Point domain to GitHub Pages
- In your domain provider, set a CNAME record:
  - Name: `www`
  - Value: `abdulwahabbadmus001-creator.github.io`
- Also set an A record for the apex domain pointing to GitHub's IPs:
  ```
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
  ```

**Step 3:** Add domain in GitHub
- Go to your repo → Settings → Pages
- Under "Custom domain", enter your domain
- Click Save
- Wait 15–30 minutes for DNS to propagate

**Step 4:** Update the app URL
- Open `index.html`, find this line (around line 11800):
  ```javascript
  const APP_URL = 'https://abdulwahabbadmus001-creator.github.io/Edupathh';
  ```
- Change it to:
  ```javascript
  const APP_URL = 'https://edupathapp.com.ng';
  ```
- Save and upload to GitHub

> ✅ All WhatsApp shares, referral links, and progress reports
> will automatically use the new domain.

---

## 📊 APP STATS (v35)

| Metric | Value |
|--------|-------|
| Questions in bank | 5,356 |
| Subjects covered | WAEC, NECO, JAMB, JSS, Primary |
| Screens | 19 |
| Features | 67+ |
| App version | v35.0 |
| Service Worker | v12.0 |
| File size (compressed) | ~668 KB |

---

## 🆘 TROUBLESHOOTING

**App not updating after upload?**
- Hard refresh: Ctrl+Shift+R (desktop) or clear browser cache
- The app may take up to 60 seconds to update on GitHub Pages
- Users with the old version will see an "Update available" bar

**Install prompt not showing?**
- Must be served over HTTPS (GitHub Pages does this automatically)
- Must be opened in Chrome (Android) or Safari (iPhone)
- Try clearing browser cache and refreshing

**Notifications not working?**
- User must tap Enable in Settings → Study Reminders
- iOS requires Safari and iOS 16.4+
- Some Android browsers block notifications — Chrome works best

**Firebase/login issues?**
- Check that the GitHub Pages domain is authorised in Firebase Console
- Go to Firebase Console → Authentication → Settings → Authorised domains
- Add: `abdulwahabbadmus001-creator.github.io`

---

*Built with ❤️ for Nigerian students | EduPath v35 | March 2026*
