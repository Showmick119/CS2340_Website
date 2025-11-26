# SpendWise GitHub Pages Website

A comprehensive, modern website showcasing the SpendWise personal finance Android application developed for CS 2340 at Georgia Tech.

## 🚀 Live Website

Visit the live website at: `https://[YOUR-USERNAME].github.io/[REPOSITORY-NAME]/`

## 📋 Overview

This website serves as a portfolio piece and comprehensive documentation of the SpendWise Android application, highlighting:

- **Architecture**: MVVM pattern with detailed explanations
- **Features**: Expense tracking, budgets, savings circles, AI chatbot, notifications
- **Development Journey**: 4 sprints with deliverables and achievements
- **Code Quality**: Testing strategy, design patterns, SOLID principles
- **Team Collaboration**: Agile/Scrum methodology

## 🛠️ Technologies Used

- **HTML5**: Semantic markup with accessibility features
- **CSS3**: Modern responsive design with CSS Grid and Flexbox
- **JavaScript**: Interactive elements, smooth scrolling, animations
- **GitHub Pages**: Static site hosting

## 📁 File Structure

```
docs/
├── index.html          # Main website file
├── styles.css          # Complete stylesheet
├── script.js           # JavaScript for interactivity
└── README.md          # This file
```

## 🚀 Deployment Instructions

### Option 1: GitHub Pages (Recommended)

1. **Push to GitHub Repository**
   ```bash
   git add docs/
   git commit -m "Add SpendWise website"
   git push origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Navigate to **Settings** > **Pages**
   - Under "Source", select branch: `main`
   - Under "Folder", select: `/docs`
   - Click **Save**

3. **Wait for Deployment**
   - GitHub will automatically build and deploy your site
   - This usually takes 1-2 minutes
   - Check the green banner for your live URL

4. **Access Your Website**
   - Your site will be available at: `https://[YOUR-USERNAME].github.io/[REPOSITORY-NAME]/`

### Option 2: Custom Domain (Optional)

1. **Add Custom Domain**
   - Go to **Settings** > **Pages**
   - Under "Custom domain", enter your domain (e.g., `spendwise.com`)
   - Click **Save**

2. **Configure DNS**
   - Add a CNAME record pointing to `[YOUR-USERNAME].github.io`
   - Wait for DNS propagation (can take up to 48 hours)

3. **Enable HTTPS**
   - GitHub Pages will automatically provision an SSL certificate
   - Check "Enforce HTTPS" once available

## 🎨 Customization

### Updating Content

1. **Edit HTML**: Modify `index.html` to update text, add sections, or change structure
2. **Edit Styles**: Modify `styles.css` to change colors, fonts, or layout
3. **Edit Functionality**: Modify `script.js` to add or change interactive features

### Color Scheme

The website uses CSS variables for easy color customization. Edit these in `styles.css`:

```css
:root {
    --primary: #4ECDC4;      /* Teal - primary brand color */
    --secondary: #FF6B6B;    /* Coral - alerts/warnings */
    --accent: #4CAF50;       /* Green - success states */
    --bg-light: #F5F5F5;     /* Light background */
    --text-dark: #333333;    /* Primary text */
}
```

### Adding Demo Video

Replace the video placeholder in `index.html` with your embedded video:

```html
<!-- Find this section in index.html -->
<div class="video-wrapper">
    <iframe 
        src="YOUR_YOUTUBE_EMBED_URL" 
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
    </iframe>
</div>
```

**YouTube Embed URL Format:**
- Go to your YouTube video
- Click "Share" > "Embed"
- Copy the URL from the `src` attribute
- Example: `https://www.youtube.com/embed/VIDEO_ID`

### Adding Images/Screenshots

1. Create an `assets` folder in `docs/`:
   ```
   docs/
   ├── assets/
   │   ├── screenshots/
   │   └── diagrams/
   ```

2. Add images to the folder

3. Reference in HTML:
   ```html
   <img src="assets/screenshots/dashboard.png" alt="Dashboard Screenshot">
   ```

### Updating GitHub Repository Link

Find and replace the GitHub link placeholders:

```html
<!-- In index.html, update this link -->
<a href="https://github.com/YOUR-USERNAME/YOUR-REPO" target="_blank">
```

## 📱 Responsive Design

The website is fully responsive and works on:
- ✅ Desktop (1920px and above)
- ✅ Laptop (1024px - 1920px)
- ✅ Tablet (768px - 1024px)
- ✅ Mobile (320px - 768px)

## ♿ Accessibility

The website includes:
- Semantic HTML5 elements
- ARIA labels where needed
- Keyboard navigation support
- Sufficient color contrast
- Reduced motion support for users with motion sensitivity

## 🔧 Local Development

To test the website locally:

### Method 1: Simple HTTP Server (Python)

```bash
# Navigate to the docs folder
cd docs/

# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then visit: `http://localhost:8000`

### Method 2: Live Server (VS Code Extension)

1. Install the "Live Server" extension in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"

### Method 3: Node.js HTTP Server

```bash
# Install http-server globally
npm install -g http-server

# Navigate to docs folder
cd docs/

# Start server
http-server
```

Then visit: `http://localhost:8080`

## 🐛 Troubleshooting

### GitHub Pages Not Showing

1. **Check Repository Settings**
   - Ensure GitHub Pages is enabled
   - Verify correct branch and folder are selected

2. **Check File Paths**
   - All files should be in the `docs/` folder
   - File names are case-sensitive

3. **Clear Browser Cache**
   - Hard refresh: `Ctrl + Shift + R` (Windows/Linux) or `Cmd + Shift + R` (Mac)

4. **Check GitHub Actions**
   - Go to the "Actions" tab in your repository
   - Look for any failed deployments

### Styles Not Loading

1. **Check File Paths**: Ensure `styles.css` and `script.js` are in the same folder as `index.html`
2. **Check Console**: Open browser DevTools (F12) and check for errors
3. **Verify File Names**: Ensure exact spelling and case sensitivity

### Mobile Menu Not Working

1. Ensure JavaScript is enabled in your browser
2. Check browser console for errors
3. Try clearing browser cache

## 📊 Performance

The website is optimized for performance:
- ✅ Minimal dependencies (no frameworks)
- ✅ Optimized CSS (single file, ~800 lines)
- ✅ Efficient JavaScript (no external libraries)
- ✅ Lazy loading for images
- ✅ Smooth animations with CSS transforms

Expected Lighthouse Scores:
- **Performance**: 95+
- **Accessibility**: 95+
- **Best Practices**: 95+
- **SEO**: 95+

## 📄 License

This website was created as part of the CS 2340 course project at Georgia Tech.

## 👥 Team

- Aazam Alam
- Showmick Das
- Suhaani Gupta
- Daanish Mehra
- Arush Yadav
- Rayeed Zaman

## 📧 Contact

For questions or issues, please contact the team through the course communication channels.

---

**Course**: CS 2340 - Objects and Design  
**Semester**: Fall 2025  
**Institution**: Georgia Institute of Technology

Built with ❤️ by the SpendWise Team

