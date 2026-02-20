# StaticShop Product Catalog API

This repository contains a static JSON API for StaticShop's product catalog, designed to be hosted on GitHub Pages.

## What I've Created

✅ **catalog.json** - A static JSON file containing:
- **Metadata**: Email (23f3000340@ds.study.iitm.ac.in) and version (0042eae5)
- **21 Products**: Each with id, name, category, price, stock, and rating
- **Aggregations**: Pre-computed statistics per category (electronics, home, sports)

## Next Steps to Deploy on GitHub Pages

1. **Initialize Git repository:**
   ```powershell
   git init
   git add .
   git commit -m "Add product catalog JSON"
   ```

2. **Create GitHub repository:**
   - Go to https://github.com/new
   - Name it (e.g., "tds-json4" or "staticshop-catalog")
   - Don't initialize with README (we already have one)

3. **Push to GitHub:**
   ```powershell
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: main (root)
   - Save

5. **Access your API:**
   Your JSON will be available at:
   ```
   https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/catalog.json
   ```

## Data Verification

- Total products: 21
- Categories: electronics (7), home (7), sports (7)
- All aggregations calculated correctly (count + inventoryValue per category)

## Tips

- Add `?v=1` to the URL to bust CDN cache if changes don't reflect
- GitHub Pages typically takes 1-2 minutes to deploy after pushing changes
- The JSON is valid and ready to use as a static API
