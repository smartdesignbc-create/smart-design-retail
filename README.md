# Smart Design™ Retail Operations Dashboard

> Enterprise-grade retail management platform — single file, zero install, open in any browser.

---

## ✨ What's Inside

A fully self-contained `index.html` that runs directly in any browser with **no server, no install, no login screen**. Open it and you're straight into the dashboard.

### Modules Included

| Module | Features |
|---|---|
| **Welcome Splash** | Animated 4-second intro screen — logo, progress bar, welcome message |
| **Dashboard** | Live KPIs, 7-day revenue chart, payment distribution pie, top products, recent activity |
| **Products** | Add · Edit · Archive · Restore · Delete — SKU, pricing, margin calculator, stock levels |
| **Inventory** | Stock-in/out movements, supplier tracking, reference numbers, low-stock alerts |
| **Sales (POS)** | Multi-item sales, VAT calculation, auto invoice numbers, refunds, customer info |
| **Cash Reconciliation** | Open/close daily register, variance detection, full history |
| **Reports & Analytics** | Live charts — monthly revenue, daily transactions, category breakdown, product ranking |
| **Archive Centre** | All archived records across every module — restore or permanently delete |
| **Notifications** | Smart alerts for low stock, mark read, notification centre |
| **Settings** | Business info, currency, tax rate, data export, audit log |
| **Share Demo** | Generate time-limited access codes (2–7 days) for customers — deactivate anytime |

---

## 🚀 Three Ways to Use This

### Option 1 — Open Locally (Instant, Zero Setup)
1. Download `index.html`
2. Double-click it
3. Splash screen plays → straight into the dashboard — done

---

### Option 2 — Deploy to Vercel (Free Live URL)

**Step 1:** Push to GitHub
```bash
git init
git add .
git commit -m "Smart Design Retail Dashboard"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/smartdesign-dashboard.git
git push -u origin main
```

**Step 2:** Deploy
1. Go to [vercel.com](https://vercel.com) → Sign in with GitHub
2. Click **New Project** → Import your repo
3. Click **Deploy** — live in under a minute

Your app is live at: `https://your-project.vercel.app`

The `vercel.json` handles all routing automatically.

---

### Option 3 — Deploy to Netlify (Drag & Drop)
1. Go to [netlify.com](https://netlify.com)
2. Drag the entire folder onto the deploy area
3. Live in seconds — free

---

## 🔗 Share Demo Feature

1. Open the app → go to **Share Demo** in the sidebar
2. Click **Generate New Link**
3. Choose 2, 3, 5, or 7 days
4. Copy the link or code → send to your customer
5. The link expires automatically
6. You can deactivate it at any time

Customers can explore every feature. They **cannot** generate their own share links.

---

## 🔐 Re-enabling Login (For Customer Handover)

The login screen is bypassed in this demo build. When you hand the app over to a paying customer:

1. Open `index.html` in any text editor
2. Find this line (around line 445):
   ```
   // DEMO MODE — Auto-login as owner
   ```
3. Follow the comment instructions to switch back to the login screen
4. Update the credentials in the `CREDS` object with the customer's own username/password

| Role | Username | Password |
|---|---|---|
| Owner | `owner` | `owner123` |
| Admin | `admin` | `admin123` |
| Staff | `staff` | `staff123` |

---

## 🎨 Customising for a Customer

| What | How |
|---|---|
| Business name, address, currency, VAT | Settings page inside the app |
| Login credentials | Find `const CREDS = {` in `index.html` |
| App branding / name | Search `Smart Design™` and replace |
| Remove Share feature | Find `{id:'share',...}` in `NAV_ITEMS` and delete |
| Re-enable login | See section above |

---

## 💾 Data Storage

All data saves in the browser's **localStorage** — persists between sessions on the same device. No server needed.

To back up: **Settings → Data & Backup → Export All Data** → downloads a `.json` file.

---

## 📁 Files in This Package

```
index.html     ← The entire application (127KB — open this)
vercel.json    ← Deployment config for Vercel/Netlify
README.md      ← This guide
```

---

## ✅ Pre-Launch Checklist

- [ ] Open `index.html` — splash plays then dashboard loads
- [ ] Test Products — add, edit, archive, restore
- [ ] Test Inventory — record stock in/out
- [ ] Test Sales — create a new sale with multiple items
- [ ] Test Cash — open then close the register
- [ ] Test Reports — generate and save a report
- [ ] Test Share Demo — generate a link, copy it
- [ ] Update business name in Settings
- [ ] Deploy to Vercel for a live URL
- [ ] Share the live URL with your customer

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Structure | Single HTML file — no build step |
| Styling | Embedded CSS with CSS variables |
| Logic | Vanilla JavaScript ES6+ |
| Charts | Chart.js (CDN) |
| Fonts | Inter via Google Fonts |
| Storage | localStorage |
| Deployment | Vercel / Netlify / any static host |

---

© 2025 Smart Design™ · All rights reserved · Proprietary — not for redistribution
