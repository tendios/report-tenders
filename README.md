# Análisis Económico de Licitaciones TI — España 2025

An interactive economic analysis report of IT public tenders in Spain for 2025, providing comprehensive insights into market trends, budget distribution, and procurement patterns.

## 🌐 Live Report

Visit the live report at: **[https://tendios.github.io/report-tenders/](https://tendios.github.io/report-tenders/)**

## 📋 Overview

This report presents a detailed economic analysis of **IT public tenders** in Spain during 2025. The interactive dashboard allows you to explore:

- 💰 **Budget Distribution** — Total tender values and budget allocation across different categories
- 📊 **Market Trends** — Temporal analysis of tender publication and award patterns
- 🏢 **Contracting Bodies** — Analysis of public entities issuing tenders
- 🏆 **Award Analysis** — Insights into tender awards and winning companies
- 📈 **Statistical Insights** — Key metrics and performance indicators

## 🎯 Report Details

- **Period Analyzed:** 2025 (full year)
- **Data Source:** Spanish public procurement platforms
- **Total Tenders:** 1,000+ IT-related public tenders
- **Categories Covered:** Software, Hardware, Services, Consulting, and more
- **Geographic Scope:** All regions of Spain

## ✨ Features

- **Interactive Filters** — Filter tenders by year, budget range, category, status, and more
- **Dynamic Charts** — Visualize data with interactive Chart.js graphs
- **Search Functionality** — Search across tender titles, contracting bodies, and companies
- **Responsive Design** — Works seamlessly on desktop, tablet, and mobile
- **Data Export** — Export filtered results for further analysis
- **Real-time Statistics** — Live calculation of totals, averages, and key metrics

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
├── index.html          # Main interactive report (self-contained with embedded data)
├── LICENSE            # MIT License
├── README.md          # This file
└── .github/
    └── workflows/
        └── deploy.yml # GitHub Actions deployment workflow
```

## 📊 Data Structure

The report includes comprehensive data for each tender:
- **Basic Info:** Title, reference number, publication date
- **Financial:** Budget amount, award value, savings percentage
- **Entities:** Contracting body, winning company
- **Classification:** Category, subcategory, procurement type
- **Status:** Published, awarded, cancelled, etc.
- **Geographic:** Region, province, municipality

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

The report is a single self-contained HTML file with embedded data. To update:

1. Edit `index.html` (update data, styling, or functionality)
2. Test locally in your browser
3. Commit and push:
   ```bash
   git add index.html
   git commit -m "Update tender data and analysis"
   git push origin main
   ```

GitHub Actions will automatically deploy your changes within a few minutes.

### Updating Tender Data

The tender data is embedded in the JavaScript section of `index.html`. Look for the `tenders` array to add or modify tender records.

## 🛠️ Technologies Used

- **HTML5** — Semantic markup and structure
- **CSS3** — Modern styling with CSS custom properties and responsive design
- **Vanilla JavaScript** — Interactive filtering, search, and data manipulation
- **Chart.js** — Dynamic data visualization and charts
- **GitHub Pages** — Static site hosting
- **GitHub Actions** — Automated deployment pipeline

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Thomas Baradel**

## 🔗 Related Links

- [Spanish Public Procurement Platform](https://contrataciondelestado.es)
- [Chart.js Documentation](https://www.chartjs.org/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

---

**Note:** This report analyzes public tender data from Spanish procurement platforms for the year 2025. Data is aggregated and anonymized for analysis purposes. For questions or updates, please contact the report maintainer.
