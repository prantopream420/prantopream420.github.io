# Portfolio Deployment Guide

Your portfolio is ready to deploy! Follow any of these free hosting options:

---

## Option 1: GitHub Pages (RECOMMENDED) ⭐

**URL after deployment:** `https://prantopream420.github.io`

### Steps:

1. **Create the repository on GitHub:**
   - Go to: https://github.com/new
   - Repository name: `prantopream420.github.io` (exact name required)
   - Description: "Personal Portfolio Website"
   - Set to **Public**
   - **DO NOT** initialize with README, .gitignore, or license
   - Click **Create repository**

2. **Push your code** (in Git Bash):
   ```bash
   cd C:/Users/HP/portfolio-site
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repository → Settings → Pages
   - Source: Deploy from branch **main**
   - Folder: **/ (root)**
   - Click Save

4. **Wait 2-3 minutes**, then visit: `https://prantopream420.github.io`

**Your site is ALREADY a git repository with everything committed and ready to push!**

---

## Option 2: Netlify (Drag & Drop)

**URL:** `https://prantopream-portfolio.netlify.app` (custom)

### Steps:

1. Go to: https://app.netlify.com/drop
2. Drag the entire `C:\Users\HP\portfolio-site` folder onto the page
3. Site deploys instantly! You get a URL like `random-name-123.netlify.app`
4. To customize the URL:
   - Go to Site settings → Change site name → `prantopream-portfolio`

**No account required for drag-and-drop!** (But sign up to keep the site permanent)

---

## Option 3: Vercel (Fast, Professional)

**URL:** `https://prantopream-portfolio.vercel.app`

### Steps:

1. Go to: https://vercel.com/new
2. Sign in with GitHub
3. Click **Import Git Repository**
4. Select `prantopream420/prantopream420.github.io`
5. Click **Deploy**
6. Done! URL is live immediately

---

## Option 4: Cloudflare Pages

**URL:** `https://prantopream-portfolio.pages.dev`

### Steps:

1. Go to: https://dash.cloudflare.com
2. Sign up / Log in
3. Go to Workers & Pages → Create application → Pages → Connect to Git
4. Authorize GitHub → Select your repository
5. Build settings: Leave empty (static site)
6. Click **Save and Deploy**

---

## Option 5: GitLab Pages

**URL:** `https://prantopream420.gitlab.io`

### Steps:

1. Create account at: https://gitlab.com
2. Create new project: `prantopream420.gitlab.io`
3. Push your code:
   ```bash
   cd C:/Users/HP/portfolio-site
   git remote add gitlab https://gitlab.com/prantopream420/prantopream420.gitlab.io.git
   git push -u gitlab main
   ```
4. Create file `.gitlab-ci.yml`:
   ```yaml
   pages:
     stage: deploy
     script:
       - mkdir .public
       - cp -r * .public
       - mv .public public
     artifacts:
       paths:
         - public
     only:
       - main
   ```
5. Push again → Site builds automatically

---

## Custom Domain (Optional)

After deploying to any platform above, you can use a custom domain like `prantopream.com`:

1. Buy domain from Namecheap ($8/year) or use Freenom (free)
2. In your hosting platform settings → Add custom domain
3. Update DNS records as instructed

---

## Files Ready to Deploy

Your portfolio directory contains:
- `index.html` — Main page
- `styles.css` — All styles (20KB)
- `script.js` — JavaScript (3.5KB)
- `images/` — Profile, albums, gallery photos
- `README.md` — Documentation

**Total size:** ~2.5MB (well under all free tier limits)

---

## Recommended: GitHub Pages

**Why:**
- Uses your existing GitHub account
- Free HTTPS certificate automatic
- URL is professional: `prantopream420.github.io`
- Easy to update: just `git push`
- Can add custom domain later for free

**Just run:** `git push -u origin main` after creating the repository!

---

## Need Help?

If you encounter any errors during deployment:
1. Check the repository exists and is named exactly `prantopream420.github.io`
2. Make sure it's set to **Public**
3. Verify GitHub Pages is enabled in Settings → Pages
4. Wait 2-3 minutes for DNS propagation

Your portfolio is ready — choose a platform and deploy! 🚀
