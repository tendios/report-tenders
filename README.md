# Accessibility Audit Report — Tendios Bid

A comprehensive accessibility audit report for the Tendios Bid application, documenting WCAG 2.1 Level AA compliance findings across 21 pages.

## 🌐 Live Report

Visit the live report at: **[https://tendios.github.io/report-tenders/](https://tendios.github.io/report-tenders/)**

## 📋 Overview

This report documents accessibility issues found during an audit of the **Tendios Bid** application ([bid.tendios.com](https://bid.tendios.com)). All findings are mapped to WCAG 2.1 success criteria and categorized by severity:

- 🔴 **Critical** — High impact issues that must be fixed first
- 🟠 **Moderate** — Significant barriers to accessibility
- 🟡 **Minor** — Low-severity issues

## 🎯 Audit Details

- **Initial Audit Date:** 3 March 2026
- **Extended Audit Date:** 4 March 2026
- **Auditor:** Thomas Baradel
- **Standard:** WCAG 2.1 Level AA
- **Pages Audited:** 21 pages across main app, settings, and application pages

## ✨ Features

- **Interactive Navigation** — Sidebar navigation with active section highlighting
- **Search Functionality** — Filter issues by keyword, page, or WCAG criterion
- **Responsive Design** — Works seamlessly on desktop, tablet, and mobile
- **Print-Friendly** — Optimized styles for printing or PDF export
- **Organized Structure** — Issues grouped by page with clear severity badges

## 🚀 Deployment

This report is automatically deployed to GitHub Pages using GitHub Actions. Any push to the `main` branch triggers a new deployment.

### Manual Deployment

If you need to deploy manually:

1. Ensure your changes are committed
2. Push to the `main` branch:
   ```bash
   git push origin main
   ```
3. GitHub Actions will automatically build and deploy to GitHub Pages

## 🔧 Local Development

To view the report locally:

1. Clone the repository:
   ```bash
   git clone git@github.com:tendios/report-tenders.git
   cd report-tenders
   ```

2. Open `index.html` in your browser:
   ```bash
   open index.html
   # or on Linux:
   xdg-open index.html
   # or on Windows:
   start index.html
   ```

Alternatively, use a local server:
```bash
# Python 3
python -m http.server 8000

# Node.js (with npx)
npx serve

# PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## 📁 Project Structure

```
report-tenders/
├── index.html          # Main report (self-contained)
├── LICENSE            # MIT License
├── README.md          # This file
└── .github/
    └── workflows/
        └── deploy.yml # GitHub Actions deployment workflow
```

## 🌍 Custom Domain Setup

To use a custom domain with GitHub Pages:

1. Go to your repository **Settings** → **Pages**
2. Under **Custom domain**, enter your domain (e.g., `report.yourdomain.com`)
3. Click **Save**
4. Add a CNAME record in your DNS provider pointing to `tendios.github.io`

Example DNS configuration:
```
Type: CNAME
Name: report (or your subdomain)
Value: tendios.github.io
TTL: 3600
```

## 📝 Updating the Report

The report is a single self-contained HTML file. To update:

1. Edit `index.html`
2. Test locally in your browser
3. Commit and push:
   ```bash
   git add index.html
   git commit -m "Update audit findings"
   git push origin main
   ```

GitHub Actions will automatically deploy your changes within a few minutes.

## 🛠️ Technologies Used

- **HTML5** — Semantic markup
- **CSS3** — Modern styling with CSS custom properties
- **Vanilla JavaScript** — Search and navigation functionality
- **GitHub Pages** — Static site hosting
- **GitHub Actions** — Automated deployment

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Thomas Baradel**

## 🔗 Related Links

- [Tendios Bid Application](https://bid.tendios.com)
- [WCAG 2.1 Guidelines](https://www.w3.org/TR/WCAG21/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

---

**Note:** This report is for internal use and documents accessibility findings as of March 2026. For questions or updates, please contact the auditor.
