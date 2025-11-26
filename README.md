# SpendWise - GitHub Pages Website

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen)](https://YOUR-USERNAME.github.io/CS2340_Website/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> A comprehensive, modern website showcasing the SpendWise personal finance Android application developed for CS 2340 (Objects and Design) at Georgia Tech.

## 🌐 Live Website

**Visit**: `https://YOUR-USERNAME.github.io/CS2340_Website/`

*(Update the URL above after deployment)*

---

## 📖 About SpendWise

SpendWise is a comprehensive personal finance management Android application that empowers users to:
- 📊 Track expenses with categories and validation
- 💰 Create and monitor budgets (weekly/monthly)
- 📈 Visualize spending with interactive charts
- 👥 Participate in group saving challenges
- 🤖 Get AI-powered financial guidance (LLaMA 3.2)
- 🔔 Receive smart notifications and reminders

**Developed by**: Aazam Alam, Showmick Das, Suhaani Gupta, Daanish Mehra, Arush Yadav, Rayeed Zaman  
**Course**: CS 2340 - Objects and Design  
**Semester**: Fall 2025  
**Institution**: Georgia Institute of Technology

---

## ⚡ Quick Start

### Option 1: Ultra-Quick (5 minutes)
See **[QUICK_START.md](QUICK_START.md)** for the fastest deployment path.

### Option 2: Comprehensive (15 minutes)
See **[DEPLOYMENT_CHECKLIST.md](DEPLOYMENT_CHECKLIST.md)** for step-by-step instructions with verification.

---

## 📁 Project Structure

```
CS2340_Website/
├── docs/                          ← GitHub Pages source
│   ├── index.html                ← Main website (850+ lines)
│   ├── styles.css                ← Complete styles (1,800+ lines)
│   ├── script.js                 ← JavaScript (400+ lines)
│   ├── README.md                 ← Detailed deployment guide
│   ├── ASSETS_GUIDE.md          ← How to add screenshots/videos
│   ├── _config.yml              ← GitHub Pages config
│   └── assets/
│       └── architecture-diagram.svg  ← MVVM diagram
├── QUICK_START.md                ← 5-minute deployment guide
├── DEPLOYMENT_CHECKLIST.md       ← Comprehensive checklist
├── PROJECT_SUMMARY.md            ← Complete project overview
└── .gitignore                    ← Git configuration
```

---

## 🚀 Deployment Instructions

### Prerequisites
- GitHub account
- Git installed
- Repository pushed to GitHub

### Steps

1. **Update Repository Links** (2 min)
   ```bash
   # Edit docs/index.html
   # Replace "https://github.com" with your actual repo URL
   ```

2. **Push to GitHub** (1 min)
   ```bash
   git add .
   git commit -m "Add SpendWise website"
   git push origin main
   ```

3. **Enable GitHub Pages** (2 min)
   - Go to **Settings** → **Pages**
   - Source: Branch `main`, Folder `/docs`
   - Click **Save**

4. **Visit Your Live Site** ✅
   - Wait 1-2 minutes
   - URL: `https://YOUR-USERNAME.github.io/CS2340_Website/`

**Detailed Instructions**: See [DEPLOYMENT_CHECKLIST.md](DEPLOYMENT_CHECKLIST.md)

---

## 📚 Documentation

| Document | Description | Time to Read |
|----------|-------------|--------------|
| [QUICK_START.md](QUICK_START.md) | Deploy in 5 minutes | 2 min |
| [DEPLOYMENT_CHECKLIST.md](DEPLOYMENT_CHECKLIST.md) | Comprehensive deployment guide | 5 min |
| [PROJECT_SUMMARY.md](PROJECT_SUMMARY.md) | Complete project overview | 10 min |
| [docs/README.md](docs/README.md) | Website customization guide | 15 min |
| [docs/ASSETS_GUIDE.md](docs/ASSETS_GUIDE.md) | Adding videos/screenshots | 10 min |

---

## ✨ Website Features

### 🎨 Design
- Modern, professional UI with gradients
- Fully responsive (mobile, tablet, desktop)
- Smooth animations and transitions
- Accessible (WCAG AA compliant)
- Fast loading (zero external dependencies)

### 📄 Content Sections
1. **Home/Introduction** - Hero, overview, key features
2. **Architecture** - MVVM pattern, design patterns, SOLID principles
3. **Features** - 7 major features with detailed explanations
4. **Demo Video** - Embedded video placeholder
5. **Development Journey** - 4 sprints timeline
6. **Code Quality** - Testing, 17 test classes
7. **Technologies** - Tech stack details
8. **Team** - All 6 members with contributions

### 🛠️ Technical
- **HTML5**: Semantic, accessible markup
- **CSS3**: Modern Grid/Flexbox layouts
- **Vanilla JavaScript**: No frameworks, optimized performance
- **SVG**: Custom architecture diagram included
- **Lighthouse Score**: Expected 95+

---

## 🎯 What's Included

✅ **Complete Website** - Ready to deploy  
✅ **Responsive Design** - Works on all devices  
✅ **Documentation** - Comprehensive guides  
✅ **Architecture Diagram** - MVVM visualization  
✅ **No Dependencies** - Pure HTML/CSS/JS  
✅ **Professional Design** - Portfolio-quality  
✅ **SEO Optimized** - Search engine friendly  
✅ **Accessibility** - WCAG compliant

---

## 📱 Screenshots

*Add screenshots of your live website here after deployment*

---

## 🔧 Customization

### Add Demo Video
```html
<!-- In docs/index.html, replace video placeholder with: -->
<iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID"></iframe>
```

### Add App Screenshots
```bash
# Create folder
mkdir docs/assets/screenshots

# Add images
# Reference in HTML: <img src="assets/screenshots/dashboard.png">
```

### Update Colors
```css
/* In docs/styles.css, modify: */
:root {
    --primary: #4ECDC4;      /* Your primary color */
    --secondary: #FF6B6B;    /* Your secondary color */
    --accent: #4CAF50;       /* Your accent color */
}
```

**Full Customization Guide**: [docs/README.md](docs/README.md)

---

## 📊 Statistics

- **Lines of Code**: 4,000+
- **Documentation**: 5 comprehensive guides
- **Sections**: 9 major content areas
- **Responsive Breakpoints**: 4 (mobile, tablet, laptop, desktop)
- **Zero Dependencies**: Pure vanilla web technologies

---

## 🎓 Educational Value

This website demonstrates:
- ✅ Software engineering principles (SOLID, GRASP)
- ✅ Design patterns (Singleton, Factory, Strategy)
- ✅ MVVM architecture
- ✅ Agile/Scrum methodology
- ✅ Testing practices
- ✅ Professional documentation
- ✅ Team collaboration
- ✅ Full-stack web development

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| 404 Error | Check GitHub Pages settings: `/docs` folder selected |
| Styles broken | Wait 2 min, hard refresh (Ctrl+Shift+R) |
| Changes not showing | GitHub Pages takes 1-5 min to update |
| Mobile menu not working | Check JavaScript console for errors |

**Full Troubleshooting**: [DEPLOYMENT_CHECKLIST.md](DEPLOYMENT_CHECKLIST.md#troubleshooting)

---

## 🌟 Key Highlights

- **Production-Ready**: Deploy immediately with zero configuration
- **Portfolio-Quality**: Professional design suitable for resumes
- **Comprehensive**: Documents entire development journey
- **Extensible**: Easy to add screenshots, videos, diagrams
- **Well-Documented**: 5 detailed guides included
- **Performance**: Optimized for speed and SEO

---

## 📞 Support

- **Deployment Issues**: See [DEPLOYMENT_CHECKLIST.md](DEPLOYMENT_CHECKLIST.md)
- **Adding Assets**: See [docs/ASSETS_GUIDE.md](docs/ASSETS_GUIDE.md)
- **Customization**: See [docs/README.md](docs/README.md)
- **GitHub Pages Docs**: https://docs.github.com/en/pages

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👥 Team

**SpendWise Development Team**:
- Aazam Alam
- Showmick Das
- Suhaani Gupta
- Daanish Mehra
- Arush Yadav
- Rayeed Zaman

**Course**: CS 2340 - Objects and Design  
**Instructor**: TBD  
**Semester**: Fall 2025  
**Institution**: Georgia Institute of Technology

---

## 🎉 Ready to Deploy!

Follow the [QUICK_START.md](QUICK_START.md) guide and have your website live in 5 minutes!

**Questions?** Check the comprehensive documentation in the `docs/` folder.

---

<div align="center">

**Built with ❤️ by the SpendWise Team**

🐝 Georgia Tech | CS 2340 | Fall 2025 🐝

[View Live Website](https://YOUR-USERNAME.github.io/CS2340_Website/) • [Report Issue](https://github.com/YOUR-USERNAME/CS2340_Website/issues)

</div>
A website displaying our work for the CS 2340 Project.
