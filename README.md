# TakaTrack — Personal Finance Tracker 💰

> A fully offline, single-file personal finance tracker built for Bangladesh — track expenses, earnings, loans, savings, and goals in **Taka (৳)**.

---

## ✨ Features

### 🏠 Home (Dashboard)
- Daily, weekly, monthly, and yearly expense totals at a glance
- Monthly budget progress bar with remaining balance
- Negative balance shown clearly when expenses exceed budget
- Today's full breakdown of all entries
- Recent transaction history
- USD total tracker (for USD-denominated expenses)
- End-of-month prompt: cover deficit from savings, or deposit surplus into an account

### ➕ Add Entry (Two Tabs)
**Expense Tab**
- Categories: Transport, Food, Shopping, Books, Loan, Lend, Extra
- Date navigation — log entries for any past or future date
- Loan entries: optionally count toward expense total; auto-tracked in Debts
- Lend entries: auto-tracked in Debts for easy follow-up
- Extra expenses support both ৳ Taka and $ USD

**Earning Tab**
- Categories: Salary, Freelance, Business, Gift, Other
- Track all income sources by date

**All Entries Panel**
- All expenses and earnings for the selected date shown together in one unified list — no switching between categories to review

### 🛡️ Debts
- Shows **all** loan and lend entries across every month — not just the current one
- 🔴 Loans — money you owe; mark as paid to remove
- 🤝 Lends — money others owe you; mark as received to clear
- Summary totals for both

### 📊 Analytics
- Monthly savings percentage based on budget
- Spending rank by category
- 6-month bar chart comparison
- Category donut chart breakdown

### 💾 Savings & Net Worth
- Bank/MFS account cards (Dutch-Bangla, bKash, Nagad, etc.)
- Deposit savings into specific accounts
- Savings history log
- Net worth = bank balances − loans
- **Saving for Goals** card — allocate a portion of your savings to specific goals using a slider
- End-of-month flow: if budget leftover, asks which account to deposit it into

### 🎯 Goals
- Create financial goals with target amount, date, priority, and monthly saving plan
- Progress bar per goal
- Days and months remaining + monthly amount needed
- Add savings to a goal manually
- Link from Savings tab — set how much of your "Saving for Goals" fund goes to each goal

---

## 🚀 Getting Started

This app is a **single HTML file** — no server, no install, no account needed.

### Run it
1. Download `TakaTrack.html`
2. Open it in any browser (Chrome recommended for best PWA support)
3. That's it — your data is stored locally in your browser

### Install as App (PWA)
On Android/Chrome:
- Tap the menu (⋮) → **Add to Home screen** → **Add**

On iOS/Safari:
- Tap Share → **Add to Home Screen**

---

## 📂 Data Storage

All data is saved in your browser's `localStorage` — nothing is sent to any server.

| Key | Contents |
|---|---|
| `ttData` | All daily expense entries |
| `ttEarnings` | All earning entries |
| `ttDebt` | Loan/lend tracker |
| `ttBanks` | Bank/MFS accounts |
| `ttSavingsHist` | Savings deposit history |
| `ttPlans` | Financial goals |
| `ttSettings` | Budget, preferences |
| `ttGoalAlloc` | Goal allocation from savings |

> ⚠️ Clearing browser data will erase everything. Use the **Export Excel** button (top-right) to back up your data regularly.

---

## 📤 Export

Tap the **export icon (📄)** in the top-right to download an `.xlsx` file with:
- All expenses sheet
- Monthly summary sheet
- Loans & Lends sheet

---

## 🛠️ Tech Stack

| | |
|---|---|
| Language | Vanilla HTML + CSS + JavaScript |
| Charts | [Chart.js 4.4](https://www.chartjs.org/) |
| Excel Export | [SheetJS (xlsx)](https://sheetjs.com/) |
| Fonts | Google Fonts — Playfair Display, DM Sans |
| Offline | Service Worker (PWA) |
| Storage | Browser localStorage |
| Dependencies | Zero npm packages, zero build step |

---

## 🗺️ Roadmap / Ideas

- [ ] Cloud sync / backup to Google Drive
- [ ] Dark mode toggle
- [ ] Recurring expense reminders
- [ ] Multiple currency conversion rates
- [ ] SMS/notification reminders for loan due dates
- [ ] Password lock / PIN protection

---

## 🤝 Contributing

This is a single-file project — all code lives in `TakaTrack.html`.

1. Fork the repo
2. Make your changes in the HTML file
3. Test in a browser (no build needed)
4. Submit a pull request

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 👤 Author

Built for personal use in Bangladesh 🇧🇩. If you find it useful, feel free to ⭐ the repo!
