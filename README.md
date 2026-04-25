# Roman Numeral Converter – Deployment Guide

## Files in this package

- `index.html` — Main converter page (the tool)
- `about.html` — About page (required for AdSense)
- `privacy.html` — Privacy Policy (required for AdSense)
- `contact.html` — Contact page (create a simple one, or use a Google Form)
- `README.md` — This file

---

## Deploy to GitHub Pages (free hosting, live URL)

### Step 1: Create a GitHub account
Go to https://github.com and sign up for free.

### Step 2: Create a new repository
1. Click the **+** in the top right → **New repository**
2. Name it something like `roman-numeral-converter`
3. Set it to **Public**
4. Click **Create repository**

### Step 3: Upload your files
1. On the repository page, click **Add file → Upload files**
2. Drag all four HTML files into the upload area
3. Click **Commit changes**

### Step 4: Enable GitHub Pages
1. Go to **Settings** (tab at top of your repo)
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Branch: **main**, folder: **/ (root)**
5. Click **Save**

### Step 5: Your site is live!
After ~60 seconds, your site will be at:
`https://YOUR-USERNAME.github.io/roman-numeral-converter/`

---

## Add a custom domain (optional, do this before applying to AdSense)

### Buy a domain
Good registrars: Namecheap (~$10/yr), Porkbun (~$8/yr)
Suggested names: `romannumeraltool.com`, `romanconvert.net`, `numeralconverter.com`

### Connect it to GitHub Pages
1. In your domain registrar's DNS settings, add a CNAME record:
   - Name: `www`
   - Value: `YOUR-USERNAME.github.io`
2. In GitHub Pages settings, enter your custom domain
3. Check "Enforce HTTPS"
4. Allow 10–30 minutes for DNS to propagate

---

## Apply for Google AdSense

1. Go to https://adsense.google.com
2. Sign up and enter your site's URL
3. Add the AdSense verification code (paste it into the `<head>` of index.html, about.html, and privacy.html)
4. Re-upload to GitHub
5. Submit for review

**Tips to get approved faster:**
- Make sure Privacy Policy and About pages are working
- Have at least 3–5 pages of content
- Add a simple contact page (link to a Google Form is fine)
- Wait until you have a custom domain before applying

### After approval: replace ad placeholders
Find these comments in `index.html` and replace the `<div>` with your AdSense code:
```
<!-- TOP AD BANNER (replace with AdSense code) -->
<!-- AD PLACEHOLDER (replace with AdSense) -->
<!-- INLINE AD (replace with AdSense) -->
```

---

## Future tools to add (subdomains or same site)

Each tool brings its own traffic. Ideas that rank well:
- Age in Days calculator (`age.yourdomain.com`)
- Binary/Decimal/Hex converter
- Word character counter
- Unix timestamp converter
- Text case converter (UPPER, lower, Title Case)
- Percentage calculator

---

## SEO tips

- Update the `<title>` and `<meta name="description">` to match real search queries
- Add your site to **Google Search Console** (free) once it's live
- Submit your sitemap: create a `sitemap.xml` with all your page URLs
- The FAQ answers target specific search queries like "what is 2025 in roman numerals" — don't delete them
