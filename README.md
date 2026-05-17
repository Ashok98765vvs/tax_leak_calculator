# 🧮 Tax Leak Calculator — US LLC + India Cross-Border Modeling

> **Educational tool only. Not tax, legal, or immigration advice.**
> Always consult a qualified US CPA and Indian CA (FEMA/export specialist) before filing.

---

## 📌 What is This?

An interactive, browser-based tax modeling calculator for founders running a **US LLC** (Wyoming or similar) while operating an **Indian entity** (SaaS / services company).

It models the combined tax exposure across both jurisdictions and shows you:
- How much tax "leaks" as a % of gross US revenue
- US federal income tax and self-employment tax
- Indian business income tax (with cess and surcharge)
- Foreign Tax Credit (FTC) savings via Form 67 / ITR-3
- After-tax cash retained


---

## 🚀 How to Run

### Option 1 — Open Directly (No Install)
1. Download `index.html`
2. Open it in any browser (Chrome, Firefox, Safari, Brave)
3. No server, no npm, no install needed ✅

### Option 2 — Clone & Open
```bash
git clone https://github.com/YOUR_USERNAME/tax-leak-calculator.git
cd tax-leak-calculator
open index.html    # macOS
start index.html   # Windows
```

---

## ⚙️ Features

| Feature | Details |
|---|---|
| **3 Scenario Presets** | Conservative, Treaty Position, Resident Fallback |
| **US LLC Inputs** | Gross revenue, India invoice, other expenses, FX rate |
| **US Tax Settings** | NRA vs Resident, SE tax toggle, treaty exemption toggle |
| **India Tax Settings** | New/Old regime, Company 22%/25%, cess, surcharge |
| **FTC Modeling** | Foreign Tax Credit savings (Form 67 / ITR-3) |
| **Live Waterfall** | Step-by-step income and tax breakdown |
| **Tax Leak Bar** | Color-coded: green < 15%, yellow < 28%, red ≥ 28% |
| **Compliance Warnings** | Transfer-pricing risk, treaty caution, SE tax, F-1 note |
| **Zero Dependencies** | Plain HTML + CSS + JavaScript — no frameworks |

---

## 🧪 Example Scenario (Default)

| Input | Value |
|---|---|
| US LLC Gross Revenue | $100,000 |
| Invoice to Indian Entity | $80,000 |
| FX Rate | ₹83 / USD |
| Filing Status | Nonresident Alien (1040-NR) |
| India Tax Rate | 25% + 4% cess |
| FTC | ON |

**Result:**
- US Federal Tax: ~$4,200
- India Tax (post-FTC): ~$19,600
- **Combined Tax Leak: ~23.8%**
- After-Tax Cash: ~$76,200

---

## 📂 File Structure
tax-leak-calculator/
│
├── index.html ← Entire app (HTML + CSS + JS in one file)
└── README.md ← This file


---

## 🔢 How the Math Works

---

## 📋 Scenario Presets Explained

### Conservative _(recommended starting point)_
- Filing: Nonresident Alien (1040-NR)
- No treaty exemption claimed
- SE tax: OFF
- FTC: ON
- Use this when you have **not confirmed treaty position** with a CPA

### Treaty Position
- Same as Conservative but **US federal tax = $0** (treaty Article-based)
- Only use if your CPA confirms treaty exemption applies to your LLC structure

### Resident Fallback
- Filing: 1040 (US Resident / Citizen)
- SE tax: ON
- No treaty
- Shows **worst-case US exposure** if you are treated as a US tax resident

---

## ⚠️ Compliance Warnings Built-in

The calculator automatically flags:
- **Transfer-pricing risk** — if India invoice exceeds 85% of US revenue
- **Treaty caution** — treaty exemption requires professional confirmation
- **SE tax note** — self-employment tax significantly increases leakage
- **FTC reminder** — Form 67 must be filed before Section 139(1) deadline
- **F-1 visa note** — F-1 visa holders generally cannot claim US-India treaty benefits

---

## 🌏 Who Is This For?

- Indian founders running a **Wyoming / Delaware LLC** for US clients
- SaaS or services founders with **Indian entity doing the actual work**
- Anyone modeling the **US LLC → India invoice** cross-border structure
- Students, indie hackers, and startup founders doing **pre-CPA planning**

---

## 🤝 Contributing

Pull requests welcome! Ideas for improvement:
- [ ] Export results to PDF / CSV
- [ ] Multi-year projection view
- [ ] DTAA treaty article selector
- [ ] INR-first mode for India-side modeling
- [ ] Dark/light theme toggle

---

## 📜 License

MIT License — free to use, fork, and modify.

---

## ❗ Disclaimer

This tool provides **illustrative scenario modeling only**.
- Numbers are approximate and depend on your specific facts
- Tax law changes frequently in both the US and India
- **Always consult a US CPA** for 1040-NR / 1040 filing decisions
- **Always consult an Indian CA** (with FEMA + export of services expertise) for ITR-3, Form 67, RBI compliance, and GST
- This tool does **not** constitute tax, legal, or immigration advice

---

*Built for cross-border founders navigating US LLC + India entity structures.*
