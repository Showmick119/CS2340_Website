# SpendWise Website Assets Guide

This document outlines the additional assets needed to complete the SpendWise website.

## 📹 Demo Video

### Required
- **Format**: YouTube or Vimeo embed, or direct MP4 file
- **Duration**: 3-5 minutes
- **Content**: 
  - App launch and authentication
  - Dashboard overview with charts
  - Creating and viewing expenses
  - Creating and tracking budgets
  - Joining a savings circle
  - Chatbot interaction with custom commands
  - Notification system demonstration
  - Date simulation functionality

### How to Add

**Option 1: YouTube Embed**
```html
<!-- In index.html, replace the video-placeholder div with: -->
<iframe 
    src="https://www.youtube.com/embed/YOUR_VIDEO_ID" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen>
</iframe>
```

**Option 2: Vimeo Embed**
```html
<iframe 
    src="https://player.vimeo.com/video/YOUR_VIDEO_ID" 
    frameborder="0" 
    allow="autoplay; fullscreen; picture-in-picture" 
    allowfullscreen>
</iframe>
```

**Option 3: Direct Video File**
```html
<video controls>
    <source src="assets/demo-video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

---

## 📊 Architecture Diagram

### Recommended Tool
Use **draw.io** (https://app.diagrams.net/) to create the MVVM architecture diagram.

### Diagram Structure

```
┌─────────────────────────────────────────────────┐
│                  VIEW LAYER                      │
│  (Activities, XML Layouts, Adapters)           │
│                                                  │
│  MainActivity, Login, Register, Dashboard,      │
│  ExpenseLog, Budgetlog, SavingCircleLog, etc.  │
└────────────────┬────────────────────────────────┘
                 │ LiveData Observers
                 │ User Interactions
                 ▼
┌─────────────────────────────────────────────────┐
│              VIEWMODEL LAYER                     │
│         (Business Logic)                        │
│                                                  │
│  LoginViewModel, ExpenseViewModel,              │
│  BudgetViewModel, SavingCircleViewModel,        │
│  DashboardAnalyticsViewModel, etc.              │
└────────────────┬────────────────────────────────┘
                 │ Data Access
                 │ Firebase Calls
                 ▼
┌─────────────────────────────────────────────────┐
│               MODEL LAYER                        │
│        (Data & Domain)                          │
│                                                  │
│  Domain Models: User, Expense, Budget,          │
│  Category, SavingCircle, etc.                   │
│                                                  │
│  Infrastructure: AnalyticsRepository,           │
│  Firebase Singleton                             │
└─────────────────────────────────────────────────┘
```

### How to Add
1. Create diagram in draw.io
2. Export as SVG or PNG (recommended size: 1200px wide)
3. Save to `docs/assets/architecture-diagram.svg`
4. Reference in HTML (optional - already described in text):
```html
<div class="architecture-diagram">
    <img src="assets/architecture-diagram.svg" alt="MVVM Architecture Diagram">
</div>
```

---

## 📱 App Screenshots

### Recommended Screenshots

Create the following screenshots from the Android app:

1. **Welcome/Login Screen** (`login.png`)
   - Shows authentication interface
   - Recommended size: 1080x2340px (or actual device dimensions)

2. **Dashboard** (`dashboard.png`)
   - Main screen with charts and budget cards
   - Shows pie chart and bar chart

3. **Expense Log** (`expense-log.png`)
   - List of expenses with categories

4. **Add Expense Form** (`add-expense.png`)
   - Form with all fields visible

5. **Budget List** (`budget-list.png`)
   - Shows multiple budgets with status indicators

6. **Budget Details** (`budget-details.png`)
   - Individual budget with progress bar and calculator

7. **Savings Circles** (`savings-circles.png`)
   - List of saving circles

8. **Circle Details** (`circle-details.png`)
   - Shows members and contributions

9. **Chatbot Interface** (`chatbot.png`)
   - Chat conversation with AI

10. **Notifications** (`notifications.png`)
    - Notification dialog with alerts

### How to Capture Screenshots

**Android Emulator:**
1. Run app in Android Studio emulator
2. Take screenshot with emulator screenshot button
3. Or use: `adb exec-out screencap -p > screenshot.png`

**Physical Device:**
1. Enable USB debugging
2. Connect device
3. Use: `adb exec-out screencap -p > screenshot.png`
4. Or use device screenshot (Power + Volume Down)

### How to Add to Website

1. Create folder: `docs/assets/screenshots/`
2. Save all screenshots there
3. Optionally add to Features section:

```html
<!-- Example: Add after feature description -->
<div class="feature-screenshot">
    <img src="assets/screenshots/dashboard.png" alt="Dashboard Screenshot">
</div>
```

---

## 📐 UML Diagrams

### Required Diagrams

From your sprint deliverables, include:

1. **Domain Model** (Sprint 1)
   - Shows classes, attributes, relationships
   - Format: PNG or SVG

2. **Use Case Diagram** (Sprint 1)
   - Shows actors and use cases
   - Format: PNG or SVG

3. **Sequence Diagrams** (Sprint 2 & 3)
   - Shows object interactions over time
   - Format: PNG or SVG

4. **Design Class Diagram (DCD)** (Sprint 3)
   - Shows detailed class structure with methods
   - Format: PNG or SVG

### How to Add

1. Create folder: `docs/assets/diagrams/`
2. Export UML diagrams from draw.io or your UML tool
3. Save with descriptive names:
   - `domain-model.png`
   - `use-case-diagram.png`
   - `sequence-expense.png`
   - `sequence-savings-circle.png`
   - `design-class-diagram.png`

4. Add to Architecture or Sprints section:

```html
<!-- Example: Add to Sprint sections -->
<div class="diagram-container">
    <img src="assets/diagrams/domain-model.png" alt="Domain Model Diagram">
    <p class="diagram-caption">Sprint 1: Domain Model with 10+ nouns</p>
</div>
```

---

## 🎨 Icons and Graphics (Optional)

### Recommended Enhancements

1. **App Icon/Logo**
   - Create SpendWise logo
   - Add to hero section
   - Format: SVG or PNG (transparent background)
   - Size: 256x256px minimum

2. **Feature Icons**
   - Currently using emojis (💰📊🤖)
   - Could replace with custom SVG icons
   - Source: https://heroicons.com/ or https://feathericons.com/

3. **Team Photos**
   - Optional: Replace avatar initials with actual photos
   - Format: Square images, 400x400px
   - Save to: `docs/assets/team/`

### How to Add Logo

```html
<!-- Replace emoji in navbar with logo -->
<div class="nav-brand">
    <img src="assets/logo.svg" alt="SpendWise Logo" class="logo-icon">
    <span class="logo-text">SpendWise</span>
</div>
```

---

## 📝 Code Snippets (Optional)

### Syntax Highlighted Code Examples

If you want to add specific code examples (like Singleton implementation):

1. Use services like Carbon (https://carbon.now.sh/) to create beautiful code images
2. Or use syntax highlighters like Prism.js

**Example: Adding Prism.js**

```html
<!-- In <head> -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/themes/prism-tomorrow.min.css">

<!-- Before </body> -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/prism.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/components/prism-java.min.js"></script>
```

Then use:
```html
<pre><code class="language-java">
public class Firebase {
    private static volatile Firebase instance;
    
    public static Firebase getInstance() {
        if (instance == null) {
            synchronized (Firebase.class) {
                if (instance == null) {
                    instance = new Firebase();
                }
            }
        }
        return instance;
    }
}
</code></pre>
```

---

## 🔗 Repository Link

### Update GitHub Link

Find all instances of placeholder GitHub links and update:

```html
<!-- Current placeholder -->
<a href="https://github.com" target="_blank">

<!-- Replace with actual repo -->
<a href="https://github.com/YOUR-USERNAME/CS2340_Website" target="_blank">
```

Files to update:
- `index.html` (navigation, hero buttons, footer)

---

## ✅ Asset Checklist

Use this checklist to track which assets you've added:

### Required
- [ ] Demo video (embedded or linked)
- [ ] GitHub repository link (updated)

### Highly Recommended
- [ ] Architecture diagram
- [ ] At least 3-5 app screenshots
- [ ] UML diagrams from sprint deliverables

### Optional
- [ ] App logo/icon
- [ ] Team member photos
- [ ] Code snippet images
- [ ] Custom feature icons

---

## 📦 Folder Structure

Recommended final structure:

```
docs/
├── index.html
├── styles.css
├── script.js
├── README.md
├── ASSETS_GUIDE.md
├── assets/
│   ├── logo.svg
│   ├── architecture-diagram.svg
│   ├── screenshots/
│   │   ├── dashboard.png
│   │   ├── expense-log.png
│   │   ├── budget-list.png
│   │   ├── savings-circles.png
│   │   └── chatbot.png
│   ├── diagrams/
│   │   ├── domain-model.png
│   │   ├── use-case-diagram.png
│   │   ├── sequence-expense.png
│   │   └── design-class-diagram.png
│   └── team/
│       ├── member1.jpg
│       └── member2.jpg
└── demo-video.mp4 (if using direct video)
```

---

## 🎯 Priority Order

1. **Update GitHub repository link** (5 minutes)
2. **Add demo video** (if available) (10 minutes)
3. **Add 3-5 key screenshots** (30 minutes)
4. **Add architecture diagram** (optional, 1 hour)
5. **Add UML diagrams** (optional, 30 minutes)
6. **Add custom logo** (optional, varies)

---

## 💡 Tips

- **Image Optimization**: Use tools like TinyPNG or Squoosh to compress images
- **Consistent Dimensions**: Keep screenshots at consistent aspect ratios
- **Alt Text**: Always add descriptive alt text for accessibility
- **File Names**: Use lowercase with hyphens (e.g., `expense-log.png`)
- **Test Locally**: Always test that images load correctly before pushing

---

For questions about adding assets, refer to the main `README.md` deployment guide.

