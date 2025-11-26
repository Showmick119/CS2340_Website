# 🚀 SpendWise Website Deployment Checklist

This checklist will help you deploy the SpendWise GitHub Pages website quickly and ensure everything is set up correctly.

## ✅ Pre-Deployment Checklist

### 1. Repository Setup
- [ ] Repository is on GitHub
- [ ] Repository is public (required for free GitHub Pages)
- [ ] All website files are in the `docs/` folder

### 2. Required Updates

#### Update GitHub Repository Links
- [ ] Open `docs/index.html`
- [ ] Search for `https://github.com` (appears in multiple places)
- [ ] Replace with your actual repository URL: `https://github.com/YOUR-USERNAME/CS2340_Website`
- [ ] Check these locations:
  - Navigation menu (line ~63)
  - Hero buttons section (line ~123)
  - Footer links (line ~891)

#### Update Team Information (Optional)
- [ ] Verify team member names in footer (line ~887-888)
- [ ] Update course semester if needed (currently "Fall 2025")

### 3. Optional Assets (Recommended)

- [ ] **Demo Video**: Add YouTube/Vimeo embed URL (line ~729-744 in index.html)
- [ ] **Screenshots**: Add app screenshots to `docs/assets/screenshots/`
- [ ] **UML Diagrams**: Add diagrams to `docs/assets/diagrams/`
- [ ] **Team Photos**: Add to `docs/assets/team/`

See `docs/ASSETS_GUIDE.md` for detailed instructions on adding assets.

## 🔧 Deployment Steps

### Step 1: Test Locally (Recommended)

Before deploying, test the website locally:

```bash
# Navigate to the docs folder
cd docs/

# Start a local server (choose one method):

# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (if installed)
npx http-server
```

Then visit `http://localhost:8000` in your browser.

**What to check:**
- [ ] All navigation links work
- [ ] Smooth scrolling works
- [ ] Mobile menu works (resize browser to mobile size)
- [ ] All sections display correctly
- [ ] Architecture diagram loads (if you see broken image, that's okay - it's optional)
- [ ] No console errors (press F12 to check)

### Step 2: Commit and Push to GitHub

```bash
# Add all files
git add docs/
git add .gitignore
git add DEPLOYMENT_CHECKLIST.md

# Commit
git commit -m "Add SpendWise GitHub Pages website"

# Push to main branch
git push origin main
```

### Step 3: Enable GitHub Pages

1. **Go to your repository on GitHub**
   - Navigate to `https://github.com/YOUR-USERNAME/YOUR-REPO`

2. **Access Settings**
   - Click the **Settings** tab (top right)

3. **Navigate to Pages**
   - In the left sidebar, click **Pages**

4. **Configure Source**
   - Under "Source", select:
     - **Branch**: `main`
     - **Folder**: `/docs`
   - Click **Save**

5. **Wait for Deployment**
   - GitHub will display a message: "Your site is ready to be published"
   - Refresh the page after 1-2 minutes
   - You should see: "Your site is published at https://YOUR-USERNAME.github.io/YOUR-REPO/"

6. **Visit Your Website**
   - Click the URL or navigate to it
   - The website should load fully

### Step 4: Verify Deployment

Visit your live website and check:

- [ ] Website loads without errors
- [ ] All sections are visible
- [ ] Navigation works
- [ ] Images load (architecture diagram, if added)
- [ ] Mobile responsive (test on phone or resize browser)
- [ ] GitHub repository link works
- [ ] Footer displays correctly

## 🐛 Troubleshooting

### Website Shows 404 Error
- **Check**: Did you select `/docs` folder in GitHub Pages settings?
- **Check**: Did you push the files to the `main` branch?
- **Fix**: Verify settings and re-save

### Styles Not Loading / Website Looks Broken
- **Check**: Are `styles.css` and `script.js` in the same folder as `index.html`?
- **Check**: Are file names correct (case-sensitive)?
- **Fix**: Verify file structure in `docs/` folder

### Architecture Diagram Shows Broken Image
- **This is okay!** The diagram is optional
- **To fix**: Ensure `docs/assets/architecture-diagram.svg` exists
- **Alternative**: Remove the diagram `<img>` tag from HTML

### Changes Not Showing Up
- **Wait**: GitHub Pages can take 1-5 minutes to update
- **Clear Cache**: Hard refresh browser (Ctrl+Shift+R or Cmd+Shift+R)
- **Check Deployment**: Go to repository → Actions tab → check build status

### Mobile Menu Not Working
- **Check**: JavaScript loading correctly (no console errors)
- **Check**: Browser JavaScript is enabled
- **Fix**: Clear browser cache and try again

## 📊 Post-Deployment

### Share Your Website
- [ ] Copy your website URL: `https://YOUR-USERNAME.github.io/YOUR-REPO/`
- [ ] Share with team members
- [ ] Add to resume/portfolio
- [ ] Submit to course if required

### Monitor Performance
- [ ] Run Lighthouse audit in Chrome DevTools
  - Open DevTools (F12)
  - Click "Lighthouse" tab
  - Click "Generate report"
  - Aim for 90+ scores in all categories

### Optional Enhancements
- [ ] Add custom domain (see `docs/README.md`)
- [ ] Add Google Analytics for tracking
- [ ] Add more screenshots/assets
- [ ] Create demo video

## 📝 Quick Reference

### File Structure
```
docs/
├── index.html              ← Main website file
├── styles.css              ← All styles
├── script.js               ← All JavaScript
├── README.md              ← Deployment guide
├── ASSETS_GUIDE.md        ← Asset instructions
├── _config.yml            ← GitHub Pages config
└── assets/
    └── architecture-diagram.svg  ← MVVM diagram
```

### Important Links
- **GitHub Repository**: `https://github.com/YOUR-USERNAME/YOUR-REPO`
- **GitHub Pages Settings**: `https://github.com/YOUR-USERNAME/YOUR-REPO/settings/pages`
- **Live Website**: `https://YOUR-USERNAME.github.io/YOUR-REPO/`
- **Local Testing**: `http://localhost:8000`

### Key Files to Update
1. `docs/index.html` - Update GitHub links (search for `https://github.com`)
2. `docs/index.html` - Add demo video embed (line ~729)
3. `docs/ASSETS_GUIDE.md` - Follow to add screenshots/diagrams

## ✨ Success Criteria

Your deployment is successful when:
- ✅ Website is accessible at your GitHub Pages URL
- ✅ All sections display correctly
- ✅ Navigation works smoothly
- ✅ Mobile responsive (test on phone)
- ✅ No console errors (F12 to check)
- ✅ GitHub repository link works

## 🎉 Congratulations!

You've successfully deployed the SpendWise website! 

### Next Steps:
1. Share the URL with your team
2. Add screenshots and demo video
3. Add to your resume/portfolio
4. Run Lighthouse audit for performance metrics

---

## 📞 Support

If you encounter issues:
1. Check `docs/README.md` for detailed troubleshooting
2. Check `docs/ASSETS_GUIDE.md` for asset instructions
3. Verify GitHub Pages build status in Actions tab
4. Clear browser cache and try again

---

**Last Updated**: November 2025  
**Created for**: CS 2340 - Objects and Design, Georgia Tech  
**Team**: SpendWise (Aazam Alam, Showmick Das, Suhaani Gupta, Daanish Mehra, Arush Yadav, Rayeed Zaman)

