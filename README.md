# Ryan Wolpert - Developer Portfolio

A modern, interactive portfolio website showcasing ML/AI and full-stack development projects. Built with vanilla HTML, CSS, and JavaScript featuring a dark theme with blue/purple accents, smooth animations, and responsive design.

![Portfolio Preview](https://via.placeholder.com/1200x600/0a0e27/6366f1?text=Your+Portfolio+Preview)

## ✨ Features

- 🎨 **Modern Dark Theme** - Sleek dark mode with gradient accents (blue/purple)
- 🚀 **Smooth Animations** - Floating cards, scroll animations, and hover effects
- 📱 **Fully Responsive** - Works perfectly on desktop, tablet, and mobile
- 🎯 **Interactive Elements** - Animated navigation, project cards, and skill tags
- ⚡ **Fast & Lightweight** - No frameworks, pure vanilla JavaScript
- 🔍 **SEO Friendly** - Semantic HTML structure
- ♿ **Accessible** - ARIA labels and keyboard navigation support

## 🚀 Quick Start

### Local Development

1. **Clone or download this repository**
   ```bash
   git clone https://github.com/rwolpert8/dev-portfolio.git
   cd dev-portfolio
   ```

2. **Open in browser**
   - Simply open `index.html` in your browser
   - Or use a local server:
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Node.js (with http-server)
     npx http-server
     ```

3. **View at** `http://localhost:8000`

## 📝 Customization Guide

### 1. Personal Information

**In `index.html`:**

- **Line 7:** Update page title
  ```html
  <title>Your Name | Your Title</title>
  ```

- **Lines 21-24:** Update navigation logo (initials)
  ```html
  <a href="#" class="nav-logo">YI</a>
  ```

- **Lines 37-42:** Update hero section name and description
  ```html
  <h1 class="hero-title">
      Hi, I'm <span class="gradient-text">Your Name</span>
  </h1>
  ```

- **Lines 52-83:** Update contact links (email, LinkedIn, GitHub, resume)

### 2. Projects

**In `index.html`, starting at line 140:**

Each project card has this structure:
```html
<div class="project-card">
    <div class="project-header">
        <div class="project-icon">🚀</div>  <!-- Change emoji -->
        <div class="project-tags">
            <span class="tag">Tech 1</span>  <!-- Add your tech -->
            <span class="tag">Tech 2</span>
        </div>
    </div>
    <h3 class="project-title">Project Name</h3>
    <p class="project-description">
        Your project description...
    </p>
    <div class="project-highlights">
        <div class="highlight-item">✓ Key feature 1</div>
        <div class="highlight-item">✓ Key feature 2</div>
    </div>
    <div class="project-footer">
        <a href="YOUR_GITHUB_LINK" class="project-link" target="_blank">
            View Code
        </a>
        <span class="project-date">Date Range</span>
    </div>
</div>
```

**To add more projects:**
- Copy an entire `<div class="project-card">...</div>` block
- Paste it within the `<div class="projects-grid">` container
- Update the content

### 3. Skills

**In `index.html`, starting at line 273:**

To add/modify skills:
```html
<div class="skill-category">
    <h3 class="skill-category-title">Category Name</h3>
    <div class="skill-items">
        <span class="skill-item">Skill 1</span>
        <span class="skill-item">Skill 2</span>
        <!-- Add more skills -->
    </div>
</div>
```

### 4. About Section

**In `index.html`, lines 128-136:**
- Update the about text to reflect your background
- Modify the statistics (projects count, technologies, graduation year)

### 5. Color Scheme

**In `styles.css`, lines 2-13:**

```css
:root {
    --bg-primary: #0a0e27;        /* Main background */
    --bg-secondary: #101629;      /* Section backgrounds */
    --bg-tertiary: #1a1f3a;       /* Card backgrounds */
    --accent-primary: #6366f1;    /* Primary accent (blue) */
    --accent-secondary: #8b5cf6;  /* Secondary accent (purple) */
    --text-primary: #e2e8f0;      /* Main text */
    --text-secondary: #94a3b8;    /* Secondary text */
    --text-muted: #64748b;        /* Muted text */
}
```

**Popular alternative color schemes:**

**Green/Cyan Tech:**
```css
--accent-primary: #10b981;
--accent-secondary: #06b6d4;
```

**Orange/Red Warm:**
```css
--accent-primary: #f97316;
--accent-secondary: #ef4444;
```

**Pink/Purple Creative:**
```css
--accent-primary: #ec4899;
--accent-secondary: #a855f7;
```

### 6. Resume Link

**In `script.js`, lines 71-79:**

1. Upload your resume to Google Drive
2. Get the shareable link (set to "Anyone with the link can view")
3. Replace the placeholder:
   ```javascript
   resumeLink.addEventListener('click', (e) => {
       e.preventDefault();
       window.open('YOUR_GOOGLE_DRIVE_LINK_HERE', '_blank');
   });
   ```

### 7. Optional Features

**Enable typing effect** (script.js, lines 88-94):
```javascript
window.addEventListener('load', () => {
    const nameElement = document.querySelector('.gradient-text');
    if (nameElement) {
        const originalText = nameElement.textContent;
        typeWriter(nameElement, originalText, 80);
    }
});
```

**Enable particle background** (script.js, line 117):
```javascript
createParticles();
```

## 🌐 Deployment

### Deploy to GitHub Pages

1. **Create a new repository** on GitHub named `your-username.github.io`

2. **Push your code:**
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio commit"
   git branch -M main
   git remote add origin https://github.com/your-username/your-username.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Source: Deploy from branch `main`
   - Folder: `/ (root)`
   - Click Save

4. **View your site** at `https://your-username.github.io`

### Deploy to Vercel

1. **Install Vercel CLI:**
   ```bash
   npm i -g vercel
   ```

2. **Deploy:**
   ```bash
   vercel
   ```

3. Follow the prompts and your site will be live!

### Deploy to Netlify

1. **Drag and drop** your project folder to [Netlify Drop](https://app.netlify.com/drop)
2. Or connect your GitHub repo for continuous deployment

## 📱 Testing Responsiveness

- **Desktop:** Default view
- **Tablet:** < 968px width
- **Mobile:** < 640px width

Test in browser DevTools (F12) → Toggle device toolbar

## 🎨 Project Structure

```
dev-portfolio/
│
├── index.html          # Main HTML file
├── styles.css          # All styles and animations
├── script.js           # Interactive features
├── resume.md           # Your resume content
└── README.md           # This file
```

## 🔧 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## 📄 License

Free to use and modify for personal portfolios. If you use this template, a credit/link back is appreciated but not required!

## 🤝 Contributing

Found a bug or want to suggest an improvement? Feel free to open an issue or submit a pull request!

## 💡 Tips

1. **Add Live Demos:** When you deploy your projects, update the project cards with "Live Demo" buttons
2. **Update Regularly:** Keep your projects and skills current
3. **SEO:** Add meta tags for better search engine visibility
4. **Analytics:** Consider adding Google Analytics to track visitors
5. **Performance:** Optimize images and consider using WebP format
6. **Accessibility:** Test with screen readers and keyboard navigation

## 📧 Contact

- **Email:** rwolpert@alum.utk.edu
- **LinkedIn:** [ryan-wolpert-utk](https://linkedin.com/in/ryan-wolpert-utk)
- **GitHub:** [rwolpert8](https://github.com/rwolpert8)

---

**Built with ❤️ by Ryan Wolpert**

*Last updated: August 2026*
