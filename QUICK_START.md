# ⚡ SpendWise Website - 5 Minute Quick Start

## 🎯 Goal
Get your SpendWise website live on GitHub Pages in 5 minutes.

## ✅ Prerequisites
- Git installed on your computer
- GitHub account
- Repository with these files already pushed

## 🚀 3 Steps to Deploy

### Step 1: Update Repository Link (2 minutes)

1. Open `docs/index.html` in your text editor
2. Press `Ctrl+F` (or `Cmd+F` on Mac) to search
3. Search for: `https://github.com`
4. Replace ALL occurrences (there are 3) with your actual repo URL:
   ```
   https://github.com/YOUR-USERNAME/CS2340_Website
   ```
5. Save the file

### Step 2: Push to GitHub (1 minute)

Open your terminal in the project folder and run:

```bash
git add .
git commit -m "Add SpendWise website"
git push origin main
```

### Step 3: Enable GitHub Pages (2 minutes)

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under "Source":
   - Branch: **main**
   - Folder: **/docs**
5. Click **Save**
6. Wait 1-2 minutes
7. Refresh the page
8. You'll see: "Your site is published at https://YOUR-USERNAME.github.io/CS2340_Website/"

## 🎉 Done!

Visit your live website at the URL shown above.

---

## 🔍 Quick Verification

Your website should have:
- ✅ Navigation menu with 8 links
- ✅ Hero section with phone mockup
- ✅ 9 major sections (Home, Architecture, Features, etc.)
- ✅ Beautiful gradients and animations
- ✅ Mobile-responsive design
- ✅ Working "Back to Top" button

---

## 📱 Test on Mobile

1. Open the website on your phone
2. Check that the hamburger menu works
3. Scroll through all sections
4. Everything should look great!

---

## ➕ Add Demo Video (Optional - 5 more minutes)

1. Upload your demo video to YouTube
2. Click "Share" → "Embed"
3. Copy the embed code
4. Open `docs/index.html`
5. Find the Demo section (around line 730)
6. Replace the placeholder `<div class="video-placeholder">` with your embed code
7. Commit and push:
   ```bash
   git add docs/index.html
   git commit -m "Add demo video"
   git push origin main
   ```
8. Wait 1-2 minutes for GitHub Pages to update

---

## 🐛 Common Issues

**Website shows 404?**
- Make sure you selected `/docs` folder in GitHub Pages settings

**Styles look broken?**
- Wait 2-3 minutes for GitHub Pages to fully deploy
- Hard refresh: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)

**Changes not showing?**
- GitHub Pages takes 1-5 minutes to update
- Clear your browser cache

---

## 📚 More Resources

- **Full Deployment Guide**: See `DEPLOYMENT_CHECKLIST.md`
- **Adding Screenshots**: See `docs/ASSETS_GUIDE.md`
- **Customization**: See `docs/README.md`

---

## 🎓 Course Submission

If submitting for CS 2340:
1. Copy your live website URL
2. Include it in your project submission
3. Ensure the GitHub repository is accessible to TAs

---

## 💡 Pro Tips

- Test locally first: `cd docs && python -m http.server 8000`
- Add screenshots for visual appeal
- Update team member info in the footer
- Check on mobile devices
- Run Lighthouse audit in Chrome DevTools for performance metrics

---

**Need Help?** Check the full documentation in `docs/README.md` or `DEPLOYMENT_CHECKLIST.md`

**Questions?** All documentation is in this repository!

---

Built for CS 2340 - Georgia Tech - Fall 2025 🐝

