# Quick Start Guide - Turkan's Portfolio Website

Welcome! This guide will help you get your portfolio website up and running quickly.

## 🚀 Step 1: View Your Website

1. **On Windows**: Double-click `index.html` to open it in your default browser
2. **On Mac/Linux**: Open `index.html` with your preferred web browser
3. Your website should load with the placeholder content

## 📸 Step 2: Replace Images

Your images are currently SVG placeholders. To use your real photos:

### Profile Photo
1. Save your profile photo as `profile.jpg` in the `images/` folder
   - Recommended size: 200x200 pixels
   - Recommended format: JPG or PNG
2. Update `index.html` line 26:
   ```html
   <img src="images/profile.jpg" alt="Turkan Mirzaliyeva - Profile Photo">
   ```

### Project Images
1. Save your project images in the `images/` folder:
   - `project1.jpg` - Logic Gates project (320x220px)
   - `project2.jpg` - Hour of AI project (320x220px)
   - `project3.jpg` - Portfolio website project (320x220px)
2. Update references in `projects.html` (lines 46, 61, 76)
3. Update references in `projects/project*.html`

## ✏️ Step 3: Update Your Information

### In `index.html`
- Line 26: Update profile photo
- Line 30-31: These stay as is (or customize)
- Line 34-37: Update introduction text

### In `about.html`
- Line 27-36: Update "About Me" section
- Line 41-48: Skills grid with descriptions
- Line 62-100: Your technical skills (already filled with your info)
- Line 105-115: Your education information
- Line 119-121: Update contact emails

### In `projects.html`
- Lines 36-50: Project 1 details
- Lines 52-66: Project 2 details
- Lines 68-82: Project 3 details

### In `projects/project*.html`
- Update detailed descriptions
- Add links to YouTube videos or GitHub repositories
- Change technologies and learnings

## 🔗 Step 4: Update Links

### Social Links (found in all pages)
Search for these links and update:
- GitHub: Replace `turkan07` with your GitHub username
- Codecademy: Replace `turkan07` with your profile username
- Email: Replace `turkan8558@gmail.com` with your email

Current links in the code:
```html
href="https://github.com/turkan07"
href="https://www.codecademy.com/profiles/turkan07"
href="mailto:turkan8558@gmail.com"
```

## 🎨 Step 5: Optional - Customize Colors

To change the website colors, edit `css/style.css`:

1. Find the `:root` section at the top (lines 1-20)
2. Change the color values:
   ```css
   :root {
       --primary-dark: #0f172a;        /* Dark background */
       --accent-blue: #3b82f6;         /* Bright blue */
       --accent-cyan: #06b6d4;         /* Cyan/turquoise */
       --accent-purple: #a855f7;       /* Purple accent */
       /* ... more colors ... */
   }
   ```
3. Save and refresh your browser to see changes

## 🌐 Step 6: Deploy Your Website

### Option A: GitHub Pages (Free & Recommended)
1. Create a GitHub account at github.com
2. Create a new repository
3. Upload all files to the repository
4. Go to Settings → Pages → Select main branch
5. Your website will be live at `username.github.io/project3`

### Option B: Netlify (Free & Easy)
1. Go to netlify.com
2. Click "New site from Git" or "Drag and drop"
3. Upload your project folder
4. Your site will be live instantly!

### Option C: Vercel (Free & Fast)
1. Go to vercel.com
2. Import your GitHub repository or drag and drop
3. Deploy in one click!

## 📝 Content Template Guide

When updating your content, use these templates:

### Project Card Update
```html
<div class="project-card" data-animate>
    <div class="project-image">
        <img src="images/projectX.jpg" alt="Project Title">
    </div>
    <div class="project-content">
        <h3 class="project-title">Your Project Title</h3>
        <p class="project-description">
            Short description of what the project is about.
        </p>
        <a href="projects/projectX.html" class="project-link">View Project →</a>
    </div>
</div>
```

### Skill Card Update
```html
<div class="skill-card">
    <div class="skill-name">Skill Name</div>
    <div class="skill-bar">
        <div class="skill-level skill-level-advanced"></div>
    </div>
    <p style="margin-top: 1rem; font-size: 0.9rem;">
        Skill description
    </p>
</div>
```

## 🐛 Troubleshooting

### Images not showing
- Check that image files are in the `images/` folder
- Verify the file names match exactly (case-sensitive)
- Use relative paths: `images/filename.jpg`

### Links not working
- Verify file paths are correct
- Use `.html` extension for internal links
- Use `../` to go up one directory level

### Website looks broken on mobile
- The site is responsive - this shouldn't happen
- Try refreshing the page (Ctrl+F5 or Cmd+Shift+R)
- Check browser width is resizing properly

### Styling not applying
- Clear browser cache (Ctrl+Shift+Delete)
- Hard refresh (Ctrl+F5)
- Check that `css/style.css` is in the correct folder

## 📱 Testing Checklist

Before deploying, test:
- [ ] Website opens correctly in browser
- [ ] All pages load (Home, About, Projects)
- [ ] All project detail pages load
- [ ] Navigation links work
- [ ] Social media links are correct
- [ ] Images display properly
- [ ] Website looks good on mobile (resize browser window)
- [ ] Hover effects work on project cards
- [ ] Animations play smoothly
- [ ] Footer appears on all pages

## 💡 Tips

1. **Test on Multiple Browsers**: Chrome, Firefox, Safari, Edge
2. **Test on Mobile**: Use browser dev tools (F12) to simulate mobile
3. **Use Descriptive Alt Text**: Helps with accessibility and SEO
4. **Keep Content Updated**: Add new projects as you complete them
5. **Backup Your Work**: Keep a local copy and commit to GitHub
6. **Use Meaningful Filenames**: Makes navigation easier
7. **Optimize Images**: Compress before uploading for faster loading
8. **Mobile First**: Check mobile experience first, then desktop

## 🚀 Next Steps

Once your site is live:
1. Share your portfolio with friends and mentors
2. Add it to your resume and LinkedIn
3. Continue updating with new projects
4. Consider adding a blog section
5. Gather feedback and improve
6. Keep learning and building!

---

## File Structure Reference

```
project3/
├── index.html              ← Start here
├── about.html              ← Update with your info
├── projects.html           ← Update project descriptions
├── README.md              ← Detailed documentation
├── QUICKSTART.md          ← This file
├── css/
│   └── style.css          ← Optional: customize colors
├── js/
│   └── script.js          ← Advanced: modify interactions
├── images/
│   ├── profile.svg        ← Replace with profile.jpg
│   ├── project1.svg       ← Replace with project1.jpg
│   ├── project2.svg       ← Replace with project2.jpg
│   └── project3.svg       ← Replace with project3.jpg
└── projects/
    ├── project1.html      ← Update project details
    ├── project2.html      ← Update project details
    └── project3.html      ← Update project details
```

---

**That's it! Your portfolio is ready to customize. Happy building! 🎉**

Need help? Check README.md for more detailed information.
