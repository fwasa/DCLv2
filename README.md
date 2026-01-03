# DebtCalculatorLab v2

Clean deployment of the debt relief calculator platform.

## Features

- 61 location-specific pages (50 US states + 9 Canadian provinces)
- FTC/FCC compliant debt relief calculator
- Schema.org structured data (FAQPage, BreadcrumbList)
- Fully static export for fast, scalable deployment
- 100% clean UTF-8 encoding (no mojibake)

## Tech Stack

- Next.js 14.2.35 (App Router)
- React 18.3.1
- Static Site Generation (SSG)
- Lucide Icons 0.562.0

## Deployment to Vercel

### Step 1: Create New GitHub Repository

1. Go to https://github.com/new
2. Repository name: `DCLv2` (or `DebtCalculatorLabV2`)
3. Choose **Private** or **Public**
4. **DO NOT** check any boxes (no README, no .gitignore)
5. Click **"Create repository"**

### Step 2: Upload Files to GitHub

**Method A: Via GitHub Web Interface**

1. In your new repository, click **"uploading an existing file"**
2. Drag ALL files and folders from the DCLv2 folder
3. Commit message: `Initial commit - DCLv2`
4. Click **"Commit changes"**

**Method B: Via Git Command Line**

```bash
cd path/to/DCLv2
git init
git add .
git commit -m "Initial commit - DCLv2"
git remote add origin https://github.com/YOUR-USERNAME/DCLv2.git
git branch -M main
git push -u origin main
```

### Step 3: Deploy to Vercel

1. Go to https://vercel.com
2. Click **"Add New Project"**
3. Import your new GitHub repository
4. Vercel auto-detects Next.js
5. Click **"Deploy"**
6. Wait 2-3 minutes
7. Your site is live!

## Project Structure

```
DCLv2/
├── src/
│   ├── app/              # Next.js App Router pages
│   ├── components/       # React components
│   └── data/            # Location data
├── public/              # Static assets (robots.txt, sitemap.xml)
├── package.json         # Dependencies
├── next.config.js       # Next.js configuration
├── .gitignore          # Git ignore rules
├── .gitattributes      # UTF-8 enforcement
└── README.md           # This file
```

## Local Development

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Open http://localhost:3000
```

## Build for Production

```bash
# Build static export
npm run build

# Output will be in the 'out/' folder
```

## Key Pages

- `/debt-calculators/` - Pillar page
- `/debt-relief-calculator/` - National tool page
- `/debt-relief-calculator/california/` - State-specific page (example)
- `/debt-relief-calculator/texas/` - State-specific page (example)
- `/debt-relief-calculator/ontario/` - Province-specific page (example)

## Compliance

- ✅ FTC-compliant language throughout
- ✅ FCC one-to-one consent for lead capture
- ✅ Quebec excluded (regulatory compliance)
- ✅ WCAG AA accessibility standards
- ✅ Schema.org markup for SEO

## License

Copyright © 2024-2025 LENURA VENTURES INC.

## Support

For deployment issues, check:
1. Vercel build logs
2. GitHub Actions (if enabled)
3. Browser console for client-side errors

All encoding issues have been resolved in this v2 release.
