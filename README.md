# Bhart Verma - Parrot OS Themed Portfolio

A modern, interactive cybersecurity portfolio with a Parrot Security OS theme. Features a simulated desktop environment with draggable windows, a working terminal, and smooth animations.

## 🎯 Features

- **Boot Animation**: Authentic Parrot OS boot sequence
- **Interactive Desktop**: Click icons to open different sections
- **Working Terminal**: Type commands to navigate the portfolio
- **Draggable Windows**: Move windows around like a real OS
- **Responsive Design**: Works on desktop and mobile devices
- **Dark Theme**: Parrot OS color scheme with cyan/green accents
- **Smooth Animations**: Professional transitions and effects

## 🚀 Quick Start

### Option 1: GitHub Pages (Recommended)

1. **Upload Files to Your Repository**
   - Create a new repository or use your existing `CyberBhart.github.io`
   - Upload these three files:
     - `index.html`
     - `styles.css`
     - `script.js`
   - Create an `assets` folder and add your `CV.pdf`

2. **Enable GitHub Pages**
   - Go to repository Settings
   - Navigate to Pages
   - Select `main` branch as source
   - Your site will be live at `https://cyberbhart.github.io/`

### Option 2: Local Testing

1. **Download Files**
   - Save all three files in the same folder
   - Create an `assets` subfolder for your CV

2. **Open in Browser**
   - Simply double-click `index.html`
   - Or use a local server:
     ```bash
     python -m http.server 8000
     ```
   - Visit `http://localhost:8000`

## 🎨 Customization Guide

### 1. Update Personal Information

**Contact Details** (in `index.html`):
```html
<!-- Search for "Contact Window" section -->
<span class="contact-value">Your Location Here</span>
<a href="YOUR_LINKEDIN_URL">linkedin.com/in/yourname</a>
<a href="YOUR_GITHUB_URL">github.com/yourname</a>
```

**Terminal Commands** (in `script.js`):
```javascript
// Update the whoami command
whoami: () => {
    return `
<span class="output-line">Your Name</span>
<span class="output-line">Your Title</span>
<span class="output-line">Location: Your Location</span>
    `;
}
```

### 2. Customize Content

**About Section**:
- Edit the "About Window" section in `index.html`
- Update stats (Years Experience, Systems Secured, etc.)

**Skills**:
- Modify skill categories and percentages in the "Skills Window"
- Adjust skill bar widths in the HTML

**Experience**:
- Update timeline items in the "Experience Window"
- Add/remove positions as needed

**Certifications**:
- Edit certification cards in the "Certifications Window"
- Mark important certs with `class="cert-card featured"`

**Tools**:
- Update tool categories and tags in the "Tools Window"

**Resources**:
- Add your GitHub project links in the "Resources Window"

### 3. Color Scheme

To change colors, edit the CSS variables in `styles.css`:

```css
:root {
    --parrot-cyan: #06d6a0;      /* Primary accent color */
    --parrot-dark: #0a0e27;      /* Background color */
    --parrot-red: #ef476f;       /* Error/warning color */
    --parrot-yellow: #ffd166;    /* Highlight color */
    --parrot-green: #18a89a;     /* Success color */
}
```

### 4. Add New Windows

1. **Add Desktop Icon**:
```html
<div class="icon-item" data-window="new-section">
    <img src="icon-url.svg" alt="New Section">
    <span>New_Section</span>
</div>
```

2. **Create Window**:
```html
<div class="window" id="new-section" style="display: none;">
    <div class="window-header">
        <span class="window-title">🎯 New Section</span>
        <div class="window-controls">
            <span class="minimize">_</span>
            <span class="maximize">□</span>
            <span class="close">✕</span>
        </div>
    </div>
    <div class="window-content">
        <div class="content-scroll">
            <h2>Your Content Here</h2>
        </div>
    </div>
</div>
```

3. **Add Terminal Command** (in `script.js`):
```javascript
newsection: () => {
    openWindow('new-section');
    return '<span class="output-line">Opening New Section...</span>';
}
```

### 5. Update Assets

**CV/Resume**:
- Replace `assets/CV.pdf` with your resume
- Or update the link in the HTML

**Profile Images**:
- Add your photo if desired
- Update icon images for a personalized touch

## 💻 Terminal Commands

Available commands when you open the terminal:

- `help` - Show all commands
- `about` - Open About Me window
- `skills` - Display Skills
- `experience` - Show Work Experience
- `certs` - List Certifications
- `tools` - Show Security Tools
- `contact` - Contact Information
- `projects` - View GitHub Projects
- `linkedin` - Open LinkedIn Profile
- `github` - Open GitHub Profile
- `clear` - Clear Terminal
- `whoami` - Display User Info
- `ls` - List Sections
- `neofetch` - System Info (fun!)

## 🎯 Terminal Easter Eggs

Try these fun commands:
- `neofetch` - Display system information with ASCII art
- `hack` - Get a special message
- `sudo` - Try elevated privileges (hint: you already have them!)
- **Konami Code**: ↑ ↑ ↓ ↓ ← → ← → B A (surprise!)

## 📱 Responsive Design

The portfolio automatically adjusts for:
- Desktop (full experience)
- Tablet (optimized layout)
- Mobile (touch-friendly interface)

## 🔧 Technical Details

**Technologies Used**:
- Pure HTML5, CSS3, JavaScript (no frameworks needed!)
- CSS Grid & Flexbox for layouts
- CSS Variables for theming
- Vanilla JavaScript for interactivity

**Browser Support**:
- Chrome/Edge (recommended)
- Firefox
- Safari
- Opera

## 🎨 Design Credits

- Inspired by Parrot Security OS
- Color palette based on Parrot OS brand guidelines
- Icons use SVG data URLs for fast loading
- Font: Fira Code (monospace) for that hacker aesthetic

## 📝 Tips for Best Results

1. **Performance**:
   - Keep images optimized and small
   - Use SVG for icons when possible
   - Minimize external dependencies

2. **SEO**:
   - Add meta tags in `<head>` section
   - Include proper title and description
   - Add Open Graph tags for social sharing

3. **Accessibility**:
   - Ensure good color contrast
   - Add alt text to images
   - Test keyboard navigation

4. **Professional Touch**:
   - Keep content concise and impactful
   - Use action verbs in experience section
   - Highlight measurable achievements
   - Proofread everything!

## 🚀 Next Steps

**Enhancements You Can Add**:
- Blog integration (link to Medium/Dev.to)
- Project showcase with screenshots
- Skills rating system
- Downloadable resources
- Contact form integration
- Analytics (Google Analytics)
- Dark/Light mode toggle
- Sound effects (optional)
- More terminal commands
- CTF writeups section

## 📧 Support

If you need help customizing:
- Open an issue on GitHub
- Check the code comments
- Refer to this README

## 📄 License

Feel free to use this template for your own portfolio! Just make it your own and give credit where it's due.

---

**Made with 💚 by Bhart Verma**
*Cybersecurity Specialist | Ethical Hacker | Threat Hunter*

🔗 [LinkedIn](https://in.linkedin.com/in/bhartverma) | [GitHub](https://github.com/CyberBhart)
