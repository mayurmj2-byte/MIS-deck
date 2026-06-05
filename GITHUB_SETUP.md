# GitHub Setup & Deployment Guide

## Step 1: Create a New GitHub Repository

1. Go to [GitHub.com](https://github.com/new)
2. **Repository name:** `mis-deck`
3. **Description:** "Professional MIS Report Generator - Create boardroom-ready PowerPoint decks in seconds"
4. **Visibility:** Public (so anyone can use it)
5. **Initialize:** Check "Add a README file" ❌ (we'll use ours)
6. Click **Create Repository**

---

## Step 2: Clone & Add Files (via Command Line)

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/mis-deck.git
cd mis-deck

# Copy files from this package
cp MIS-Deck-Generator-Complete.html index.html
cp README.md .
cp LICENSE .
cp .gitignore .

# Create docs folder (optional)
mkdir docs
# Add documentation files here if desired
```

---

## Step 3: Push to GitHub

```bash
# Initialize git tracking
git add .
git commit -m "Initial commit: MIS Deck Generator v3.0"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/mis-deck.git
git push -u origin main
```

---

## Step 4: Enable GitHub Pages (Free Hosting)

1. Go to your repository: `https://github.com/YOUR_USERNAME/mis-deck`
2. Click **Settings** (gear icon)
3. Scroll down to **"Pages"** section on left sidebar
4. Under **"Source"**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes for deployment

---

## Step 5: Your Live URL

Once GitHub Pages deploys, your tool will be live at:

```
https://YOUR_USERNAME.github.io/mis-deck/
```

**Example:** If your GitHub username is `mayurjain`:
```
https://mayurjain.github.io/mis-deck/
```

---

## Step 6: Share & Promote

### Update Repository Description
- Add this as description: "Professional MIS Report Generator - 5 data modules, 7-slide decks, 100% browser-based"
- Add website URL: `https://YOUR_USERNAME.github.io/mis-deck/`

### Add Topics (Tags)
In repository settings, add these topics:
- `mis-deck-generator`
- `powerpoint-generator`
- `finance-tools`
- `fpa`
- `management-accounting`
- `excel-to-pptx`
- `financial-reporting`

### Create a Quick Link (Short URL)
Consider using a URL shortener for easy sharing:
```
https://bit.ly/mis-deck-generator
```

---

## Step 7: Verify Deployment

1. Go to `https://YOUR_USERNAME.github.io/mis-deck/`
2. The MIS Deck Generator should load immediately
3. Try uploading sample data
4. Generate a test PowerPoint deck

---

## Step 8: Update GitHub About Section

In your GitHub profile settings, add:
- **Bio:** "Finance Professional | Creator of MIS Deck Generator"
- **Company:** Your company name
- **Location:** Your location
- **Website:** Link to your portfolio or website

---

## Continuous Updates (Optional)

### When you add new features:

```bash
# Make changes to index.html
git add index.html
git commit -m "Feature: Add new report type"
git push origin main
```

Changes deploy automatically to GitHub Pages!

---

## Troubleshooting

### 404 Error on Pages?
- Ensure `index.html` is in the root directory
- Wait 5 minutes for Pages to rebuild
- Check Settings → Pages → Deployment status

### Outdated Version Showing?
- Hard refresh: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)
- Clear browser cache

### CDN Scripts Not Loading?
- Check browser console (F12) for errors
- Verify internet connection
- Try a different browser

---

## Repository Structure (After Setup)

```
mis-deck/
├── index.html                          ← Main tool (all-in-one file)
├── README.md                           ← Documentation
├── LICENSE                             ← MIT License
├── .gitignore                          ← Git ignore rules
└── docs/                               ← Optional documentation folder
    ├── USAGE.md
    ├── CHANGELOG.md
    └── SCREENSHOTS/                    ← Optional: Add UI screenshots
```

---

## Analytics & Tracking (Optional)

To track usage, consider adding Google Analytics:

Add this before `</body>` in index.html:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_GA_ID');
</script>
```

---

## Support & Contact Links

Update the footer with your actual contact information:
- Email
- Twitter/LinkedIn
- Website
- Phone (optional)

---

## Success! 🎉

Your MIS Deck Generator is now live and accessible worldwide!

**Share the link:** `https://YOUR_USERNAME.github.io/mis-deck/`

Every time someone uses it, they'll create professional MIS reports in minutes. 

---

**Questions? Issues? Create a GitHub Issue in your repository!**
