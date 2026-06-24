# Smart Design™ Retail Operations Dashboard

> Enterprise-grade retail management platform — single file, zero install, open in any browser.

---

## ✨ What's Inside

A fully self-contained `index.html` that runs directly in any browser with **no server, no install, no dependencies to download**. Everything is built in — styles, logic, charts, animations, and data storage.

### Modules Included

| Module | Features |
|---|---|
| **Welcome Splash** | Animated 4-second intro screen with logo, progress bar, welcome message |
| **Secure Login** | 3 role tiers — Owner, Admin, Staff — with different permissions |
| **Dashboard** | Live KPIs, 7-day revenue chart, payment distribution pie, top products, recent activity |
| **Products** | Add · Edit · Archive · Restore · Delete — with SKU, pricing, margin calculator, stock levels |
| **Inventory** | Stock-in/out movements, supplier tracking, reference numbers, low-stock alerts |
| **Sales (POS)** | Multi-item sales, VAT calculation, auto invoice numbers, refunds, customer info |
| **Cash Reconciliation** | Open/close daily register, variance detection, full history |
| **Reports & Analytics** | Live charts — monthly revenue, daily transactions, category breakdown, product ranking |
| **Archive Centre** | All archived records across every module — restore or permanently delete |
| **Notifications** | Smart alerts for low stock, mark read, notification centre |
| **Settings** | Business info, currency, tax rate, data export, audit log, danger zone |
| **Share Demo** | Owner-only — generate time-limited access codes (2–7 days), deactivate anytime |

---

## 🚀 Three Ways to Use This

### Option 1 — Open Locally (Instant)
1. Download `index.html`
2. Double-click it
3. It opens in your browser — done

Login with: `owner` / `owner123`

---

### Option 2 — Deploy to Vercel (Live URL, Free)

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
3. Click **Deploy**

Your app is live at: `https://your-project.vercel.app`

The `vercel.json` in this folder handles everything automatically.

---

### Option 3 — Deploy to Netlify (Drag & Drop)
1. Go to [netlify.com](https://netlify.com)
2. Drag the entire folder onto the deploy area
3. Live in seconds

---

## 🔐 Login Credentials

| Role | Username | Password | Permissions |
|---|---|---|---|
| **Owner** | `owner` | `owner123` | Full access + Share Demo feature |
| **Admin** | `admin` | `admin123` | All modules except Share |
| **Staff** | `staff` | `staff123` | Sales, inventory, notifications |

> ⚠️ Change these before handing to a customer. Credentials are in the `CREDS` object near the top of `index.html`.

---

## 🔗 Share Demo Feature (Owner Only)

1. Log in as **owner**
2. Click **Share Demo** in the sidebar
3. Click **Generate New Link**
4. Choose 2, 3, 5, or 7 days
5. Copy the link or the code and send to your customer
6. The link expires automatically
7. You can deactivate it at any time

Customers can explore every feature. They **cannot** generate their own share links.

---

## 🎨 Customising for a Customer

### Change Business Details
Log in → Settings → Business Info → update name, address, currency, VAT rate → Save

### Change Login Credentials
Open `index.html` in a text editor → find `const CREDS = {` near the top → update usernames and passwords

### Change the App Name / Branding
Search `Smart Design™` in `index.html` and replace with your customer's brand name

### Remove the Share Feature (after handover)
Find `{id:'share', ...}` in the `NAV_ITEMS` array and delete that line

### Change Currency
Settings → Currency field → select your currency → update symbol → Save

---

## 💾 Data Storage

All data is saved in the browser's **localStorage** — it persists between sessions on the same browser/device. No server required.

To back up data: **Settings → Data & Backup → Export All Data** — downloads a `.json` file.

---

## 📁 Files in This Package

```
index.html     ← The entire application (open this)
vercel.json    ← Deployment config for Vercel
README.md      ← This guide
```

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Structure | Single HTML file |
| Styling | Embedded CSS with CSS variables |
| Logic | Vanilla JavaScript (ES6+) |
| Charts | Chart.js (loaded from CDN) |
| Fonts | Inter via Google Fonts |
| Storage | localStorage |
| Deployment | Vercel / Netlify / any static host |

---

## ✅ Pre-Launch Checklist

- [ ] Open `index.html` and test all modules
- [ ] Log in as owner, admin, and staff to verify permissions
- [ ] Update business name and details in Settings
- [ ] Test: add a product → record stock → make a sale → reconcile cash → generate report
- [ ] Generate a share demo link and test it
- [ ] Change credentials before customer handover
- [ ] Deploy to Vercel/Netlify for a live URL
- [ ] Share the live URL with your customer

---

## 📄 License

© 2025 Smart Design™. All rights reserved.  
Proprietary software — not for redistribution without permission.

---

*Built with Smart Design™ — Enterprise Retail Management*
