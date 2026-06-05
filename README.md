# MIS Deck Generator

**A complete, professional Management Information System (MIS) reporting tool that generates boardroom-ready PowerPoint decks in seconds.**

**Made by CA Mayur Jain** | For Finance Professionals | CFO, FP&A, Management Accounting

---

## 🎯 Overview

MIS Deck Generator is a **browser-based tool** that transforms raw business data into beautifully formatted PowerPoint presentations. No server, no sign-ups, no data leaves your browser.

### Features

✅ **5 Data Modules:**
- 📈 Sales & Revenue
- 🎯 KPIs (Operations)
- 💰 Finance / P&L
- 📊 Accounts Receivable (AR Ageing)
- 📦 Stock Cover Analysis

✅ **7-Slide Professional Deck** with:
- Title slide with key metrics
- Sales performance & regional breakdown
- KPI dashboard (8 cards, colour-coded)
- Finance P&L analysis
- AR ageing breakdown
- Stock cover & inventory analysis
- Executive summary with smart alerts

✅ **Template Downloads**
- One-click download of Excel templates
- Pre-structured with sample data
- Fill in, upload, generate

✅ **8 Critical Bugs Fixed**
- Division by zero protection
- Negative value handling
- Large number formatting
- Lower-is-better KPI logic
- Header normalization
- Hex colour integrity
- Object corruption prevention
- Empty dataset graceful handling

---

## 🚀 Quick Start

### Online (No Installation)
1. Open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge)
2. Download templates for your data modules
3. Fill in your data in Excel
4. Upload CSVs or XLSX files
5. Click **Generate PowerPoint Deck** → Instant download

### Local Setup (Optional)
```bash
git clone https://github.com/yourusername/mis-deck.git
cd mis-deck
# Open index.html in your browser
```

---

## 📋 Data Templates

### Sales & Revenue
**Required:** Month, Revenue  
**Optional:** Target, Region, Product

### Operations / KPIs
**Required:** KPI, Actual  
**Optional:** Target, Unit

### Finance / P&L
**Required:** Revenue  
**Optional:** Month, COGS, Opex, EBITDA

### Accounts Receivable (AR Ageing)
**Required:** Customer, Outstanding  
**Optional:** 0-30 days, 31-60 days, 61-90 days, 90+ days, Notes

### Stock Cover
**Required:** Product, Current Stock, Avg Monthly Usage  
**Optional:** Unit Price, Unit, Reorder Level, Notes

---

## 📊 Stock Cover Calculation

The tool automatically calculates **how many months your current inventory can cover**:

```
Stock Cover (Months) = Current Stock / Avg Monthly Usage
```

**Example:**
- Current Stock: 5,000 units
- Avg Monthly Usage: 2,000 units
- **Cover: 2.5 months**

Smart alerts identify products with <2 months cover in the summary slide.

---

## 📁 File Structure

```
mis-deck/
├── index.html              (Main tool - all-in-one file)
├── README.md              (This file)
├── LICENSE                (MIT License)
├── .gitignore
└── docs/
    ├── USAGE.md           (Detailed usage guide)
    ├── CHANGELOG.md       (Version history & fixes)
    └── TEMPLATES/         (Excel template examples)
```

---

## 🔧 Technical Stack

- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **Charting:** PptxGenJS v3.12.0
- **Data Parsing:** SheetJS v0.18.5
- **No Backend Required** — Everything runs in the browser

### CDN Dependencies
```html
<script src="https://cdn.jsdelivr.net/npm/xlsx@0.18.5/dist/xlsx.full.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/pptxgenjs@3.12.0/dist/pptxgen.bundle.js"></script>
```

---

## 🎨 Slides Generated

| # | Slide | Content |
|---|-------|---------|
| 1 | Title | Company name, period, key metrics (Revenue, EBITDA, Margin %) |
| 2 | Sales | Monthly revenue vs target, regional breakdown pie chart |
| 3 | KPI Dashboard | 8 colour-coded KPI cards (green/amber/red status) |
| 4 | Finance P&L | Revenue/COGS/Opex/EBITDA trends + margin line chart |
| 5 | AR Ageing | Receivables by age bucket + top debtors list |
| 6 | Stock Cover | Inventory cover in months + valuation + reorder alerts |
| 7 | Summary | 3 key takeaways with smart risk detection |

---

## 🔐 Privacy & Security

✅ **Zero Data Collection** — All processing happens in your browser  
✅ **No Server Backend** — No data transmitted to any server  
✅ **No Cookies or Tracking** — Completely private  
✅ **Offline Capable** — Works without internet after first load

---

## 🐛 Bug Fixes (v3.0)

| Issue | Fix |
|-------|-----|
| Division by zero on zero-target KPIs | `safeDiv()` returns 0% instead of Infinity |
| Negative EBITDA bars clipped at 0 | `valAxisMinVal` set to pad 20% below minimum |
| Large numbers overflowing text boxes | `fmt()` formatter: $6.6M / $320K notation |
| "Lower-is-better" KPIs always red | `LOWER_BETTER` set inverts colour logic |
| Lowercase CSV headers not detected | `normalise()` normalizes all keys before matching |
| Hex colours with # prefix corrupt chart XML | All hex values stored without # prefix |
| Reused shadow objects corrupt file | Fresh shadow object per shape |
| Empty dataset crash | Slides skip gracefully with row-count guard |

---

## 💻 Browser Support

| Browser | Support |
|---------|---------|
| Chrome | ✅ Full Support |
| Firefox | ✅ Full Support |
| Safari | ✅ Full Support |
| Edge | ✅ Full Support |
| IE 11 | ⚠️ Limited (No ES6) |

---

## 📝 Usage Example

```
1. Launch tool: index.html
2. Download templates from "Download Templates" tab
3. Fill Sales template:
   Month,Revenue,Target,Region,Product
   Jan-25,1000000,950000,North,Widget A
   Feb-25,1100000,1000000,South,Widget B
   
4. Upload sales.csv in Upload Data tab
5. Set Company Name: "Acme Corp"
6. Set Report Month: "February 2025"
7. Click "Generate PowerPoint deck"
8. Download: MIS_acme_corp_February-2025.pptx
```

---

## 📖 Documentation

- **[USAGE.md](docs/USAGE.md)** — Detailed step-by-step guide
- **[CHANGELOG.md](docs/CHANGELOG.md)** — Version history & feature additions
- **[TEMPLATES/](docs/TEMPLATES/)** — Sample Excel files

---

## 🤝 Contributing

Found a bug? Have a feature request? 
- Open an issue on GitHub
- Submit a pull request with improvements
- Email: contact@mayurjain.in

---

## 📄 License

MIT License — Free to use, modify, and distribute

**Copyright © 2025 CA Mayur Jain**

See [LICENSE](LICENSE) for full terms.

---

## 🎓 About CA Mayur Jain

CA Mayur Jain is a Chartered Accountant specializing in:
- Financial Planning & Analysis (FP&A)
- Management Accounting
- Business Intelligence
- Financial Reporting & Compliance

**This tool was created to help finance professionals generate professional MIS reports in minutes, not hours.**

---

## 📞 Support & Contact

- 🌐 Website: www.mayurjain.in
- 📧 Email: hello@mayurjain.in
- 🐦 Twitter: @mayurjain_ca
- 💼 LinkedIn: linkedin.com/in/mayurjain

---

## 🎉 What's New (v3.0)

✨ **Stock Cover Module** — Automatically calculate how many months inventory can cover sales  
✨ **AR Ageing Analysis** — Receivables age breakdown with risk detection  
✨ **5 Data Modules** — Sales, KPI, Finance, AR, Stock  
✨ **7-Slide Decks** — Professional boardroom-ready presentations  
✨ **Smart Alerts** — Auto-detection of low stock, overdue receivables, margin pressure  
✨ **No Backend** — 100% browser-based, zero data sharing  

---

**Made with ❤️ for Finance Professionals**

*Last Updated: June 5, 2025*
