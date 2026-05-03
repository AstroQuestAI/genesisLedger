# 🔷 LEDGER — Syndicate Financial System
### సిండికేట్ ఫైనాన్షియల్ సిస్టమ్

> A cyberpunk-styled financial management web app for syndicates — scan receipts, track payments, manage partners and generate reports. All in a single HTML file.
>
> సిండికేట్‌ల కోసం సైబర్‌పంక్ స్టైల్ ఫైనాన్షియల్ మేనేజ్‌మెంట్ వెబ్ యాప్ — ఒకే HTML ఫైల్‌లో.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-00f0ff?style=for-the-badge&logo=github)](https://yourusername.github.io/reponame)
![Version](https://img.shields.io/badge/Version-1.1.0-ff24e4?style=for-the-badge)
![No Install](https://img.shields.io/badge/No%20Install-Single%20HTML%20File-34d399?style=for-the-badge)
![AI Powered](https://img.shields.io/badge/AI-Claude%20Powered-eeff96?style=for-the-badge)

---

## ✨ Features / ఫీచర్లు

| Feature | Description |
|---------|-------------|
| 🤖 **AI Receipt Scanning** | Upload any image or PDF — Claude AI extracts merchant, amount, invoice date, reference & payee automatically |
| 💰 **Cash Entry Policy** | Manual text entries blocked; cash transactions require admin approval only |
| 🔍 **Duplicate Detection** | Flags identical entries within 3 days automatically |
| 💾 **SQLite Persistence** | All data saved in browser via WebAssembly SQLite + localStorage |
| 👥 **Partner Contributions** | Track how much each partner paid to each category (Wk / Mo / All) |
| 🏷️ **Dynamic Categories** | Admin can create, rename, disable or delete categories anytime |
| 📊 **Reports + Sparkline** | Category reports with cumulative growth chart over 8 weeks |
| 🎨 **18 Themes** | 10 dark + 8 light themes, with accent, background & text colour dropdowns |
| 🔐 **Security Toggles** | Biometric unlock, 2FA, PIN lock, auto-lock settings |

---

## 📱 Screens / స్క్రీన్‌లు

```
Home        →  Project total, contribution card, quick scan actions, partner list
Ledger      →  Chat-style feed, AI scan, payee picker, cash approval, duplicates
Reports     →  Category tabs, person dropdown, received totals, partner breakdown
Analytics   →  Payee breakdown (Wk/Mo/All), totals by type, partner contributions
Admin       →  Personnel directory (CRUD), activate/disable, category manager
Settings    →  Themes, colours, font size, security, notifications, data reset
```

---

## 🚀 Quick Start / త్వరగా ప్రారంభించండి

### Option 1 — Open locally
```bash
# Just double-click index.html in Chrome, Firefox, Safari or Edge
# No installation or server needed
```

### Option 2 — GitHub Pages (recommended)
```bash
git clone https://github.com/yourusername/reponame
cd reponame
# Replace index.html with the latest build
git add index.html
git commit -m "deploy"
git push
# Enable GitHub Pages: Settings → Pages → main branch
```

### Option 3 — Netlify Drop
Drag `index.html` onto [app.netlify.com/drop](https://app.netlify.com/drop) → live URL in 30 seconds.

---

## 📄 Scanning a Receipt / రసీదు స్కాన్ చేయడం

1. Tap **Scan** (📷) on the Ledger screen or **Add Entry** on Home
2. Select who the payment was made to (category + person) or tap SKIP
3. Pick any image, screenshot or PDF from your device
4. Claude AI reads the document and extracts all transactions
5. Review the card — tap **LOG IT** to confirm
6. Contribution totals and Reports update instantly

---

## 💵 Cash Transactions / నగదు లావాదేవీలు

Type any cash-related keyword in the Ledger input bar:
- A `◆` pending card appears
- Navigate to **Admin** screen to **APPROVE** or **REJECT**
- On approval: confirmed with a filled maroon `₵` circle marker

---

## 📊 Reports Screen / రిపోర్ట్స్ స్క్రీన్

Select any category tab → choose period (Week / Month / All):

- **Total Received card** — combined totals for the whole category with sparkline chart
- **Person Dropdown** — filter to a specific individual's amounts
- **Paid by Partners** — each partner's share (Wk / Mo / All) for the selected category or person

---

## 🏷️ Category Management / కేటగిరీ మేనేజ్‌మెంట్

**Admin → CATS button:**

- View all categories with icon, colour and type (Payer / Receiver)
- 👁 Toggle to hide a category from all pills, dropdowns and tabs instantly
- ➕ Add custom category: name + colour swatch + icon → **ADD CATEGORY**
- 🗑️ Delete custom categories (people move to *Others* automatically)
- System categories (Partners etc.) are protected and cannot be deleted

---

## 🎨 Themes / థీమ్‌లు

| Dark Themes | Light Themes |
|-------------|--------------|
| Cyber · Midnight · Forest · Ember | Snow · Paper · Blossom · Sage |
| Ocean · Gold · Violet · Crimson | Sand · Lavender · Sky · Peach |
| Rose · Teal | |

Settings also include independent controls for **Accent Colour** (12 options), **Background** (22 presets), and **Text Colour** (10 options).

---

## 🔐 Security / సెక్యూరిటీ

| Toggle | Description |
|--------|-------------|
| Biometric Unlock | Face ID or Touch ID |
| Two-Factor Auth | Authenticator app required |
| PIN Lock | 4-digit fallback PIN |
| Auto Lock | Lock after 5 min inactivity |
| Cash Entry Alerts | Notify admin for cash transactions |

---

## ⚙️ Technical Details / సాంకేతిక వివరాలు

- **Single file** — all code, styles and logic in one `~210KB` HTML file
- **No framework** — pure vanilla JavaScript (no React / Vue / Angular)
- **SQLite** via `sql.js` (WebAssembly) — stored in browser `localStorage` as base64
- **AI extraction** — calls Anthropic Claude API (internet required for scanning)
- **Canvas sparkline** — drawn with native HTML5 Canvas API
- **Fonts** — Space Grotesk + Inter + Material Symbols from Google CDN

---

## 📁 Repository Structure

```
/
└── index.html    ← The entire app (single file, ~210KB)
└── README.md     ← This file
```

---

## 🇮🇳 తెలుగు సంక్షిప్త గైడ్

| స్క్రీన్ | వివరణ |
|---------|-------|
| హోమ్ | ప్రాజెక్ట్ మొత్తం, కాంట్రిబ్యూషన్ కార్డ్, పార్ట్‌నర్ లిస్ట్ |
| లెడ్జర్ | రసీదు స్కాన్, చెల్లింపు గ్రహీత ఎంపిక, నగదు ఆమోదం |
| రిపోర్ట్స్ | కేటగిరీ వారీగా స్వీకరించిన మొత్తాలు, పార్ట్‌నర్ వాటా |
| అనలిటిక్స్ | చెల్లింపు గ్రహీత వివరాలు, వారం/నెల/మొత్తం కాలమ్‌లు |
| అడ్మిన్ | సిబ్బంది డైరెక్టరీ, కేటగిరీ మేనేజ్‌మెంట్ |
| సెట్టింగ్స్ | థీమ్‌లు, రంగులు, సెక్యూరిటీ, డేటా రీసెట్ |

**రసీదు స్కాన్ చేయడం:** లెడ్జర్ → Scan బటన్ → వ్యక్తి ఎంచుకోండి → ఫైల్ సెలెక్ట్ → AI స్వయంచాలకంగా డేటా వెలికితీస్తుంది → LOG IT నొక్కండి.

**నగదు లావాదేవీలు:** టెక్స్ట్ బార్‌లో టైప్ చేయండి → Admin స్క్రీన్‌లో APPROVE/REJECT చేయండి.

---

## 📄 License

MIT — free to use, modify and distribute.

---

<div align="center">

**Ledger v1.1** · Made in India 🇮🇳 · Built with [Claude AI](https://claude.ai)

</div>
