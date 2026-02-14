# Christopher Clarke - Academic Website

A modern, professional academic website with separate pages for research and teaching, deployed via GitHub Pages.

## 🎯 Overview

This redesigned website features:
- **Modern, Clean Design**: Professional academic aesthetic with Avenir typography
- **Multi-Page Structure**: Separate pages for home, research, and teaching
- **Comprehensive Research Page**: 55+ publications, grants, PhD students, professional activities
- **Featured Publications**: Landing page highlights 5 recent papers
- **Fully Responsive**: Works beautifully on desktop, tablet, and mobile devices
- **Easy Maintenance**: Organized structure with external CSS/JS files

## 📁 File Structure

```
your-repository/
├── index.html          # Landing page with featured publications
├── research.html       # Complete research: publications, grants, students, activities
├── teaching.html       # Teaching experience and service
├── styles.css          # All website styles (Avenir font)
├── script.js           # Navigation and interaction scripts
├── img/
│   ├── chris.png      # Your profile photo
│   └── logo.png       # Logo image
├── CNAME              # Custom domain configuration
├── favicon.ico        # Website icon
└── README.md          # This file
```

## 🚀 Quick Start - Deploying to GitHub Pages

1. **Create/Update Repository**
   - If using custom domain: name it anything (e.g., `website`)
   - If using GitHub domain: name it `yourusername.github.io`

2. **Upload All Files**
   - Upload all HTML files (index.html, research.html, teaching.html)
   - Upload styles.css and script.js
   - Upload the `img/` folder with your photos
   - Upload CNAME and favicon.ico

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` → `/` (root)
   - Click Save

4. **Configure DNS (for christopherclarke.net)**
   - Your CNAME file contains: `christopherclarke.net`
   - In your domain registrar's DNS settings, add:
     - A records: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153

Your site will be live at `https://christopherclarke.net` in a few minutes!

## 📝 How to Update Your Website

### Adding New Publications

#### To Featured Publications (Landing Page)

**File**: `index.html`  
**Location**: Find "Featured Publications" section

```html
<div class="publication-item featured">
    <div class="publication-title">Your New Paper Title</div>
    <div class="publication-authors">Author 1, <strong>Clarke, Christopher</strong>, Author 3</div>
    <div class="publication-venue">Conference Name, 2025</div>
</div>
```

**Tip**: Keep only 5 featured publications. Remove the oldest when adding a new one.

#### To Complete Publications List

**File**: `research.html`  
**Location**: Find the Publications section and appropriate year

```html
<div class="publication-item">
    <div class="publication-title">Complete Paper Title</div>
    <div class="publication-authors">All authors, <strong>Clarke, Christopher</strong>, more authors</div>
    <div class="publication-venue">Full Conference/Journal Name, 2025</div>
</div>
```

Create new year heading if needed:
```html
<h3 class="year-heading">2026</h3>
```

### Adding Research Grants

**File**: `research.html`  
**Location**: Find the "Research Grants" section

```html
<div class="grant-item">
    <div class="grant-title">Grant Title or <a href="url">Link to Grant</a></div>
    <div class="grant-funder">Funding Organization Name</div>
    <div class="grant-amount">Total Awarded: £XXX,XXX</div>
</div>
```

### Adding PhD Students

**File**: `research.html`  
**Location**: Find the "PhD Student Supervision" section

```html
<div class="student-item">
    <div class="student-name"><a href="profile-url">Student Name</a></div>
    <div class="student-topic">"Research Topic Title"</div>
    <p>Co-supervised with <a href="url">Dr. Supervisor Name</a>.</p>
</div>
```

### Updating Professional Activities

**File**: `research.html`  
**Location**: Find the "Professional Activities" section

Add to appropriate subsection:
```html
<li><strong>Conference/Journal Name</strong> - Role Description</li>
```

### Updating Teaching Information

**File**: `teaching.html`  
**Location**: Find relevant section

```html
<li class="course-item">
    <strong>Course Code: Course Name</strong>
    <em>Year Range</em>
    <p>Course description.</p>
</li>
```

### Updating Your Photo

1. Replace `img/chris.png` with your new photo
2. Recommended size: 600x600 pixels or larger
3. Keep filename as `chris.png` or update all references in HTML

### Updating Contact Information

**File**: `index.html`  
**Location**: Contact section

Your current email is: **chrisclarke@acm.org**

Update as needed in the contact grid.

## 🎨 Customizing the Design

### Changing Colors

**File**: `styles.css`  
**Location**: `:root` section at top

```css
:root {
    --color-primary: #1a1a2e;      /* Main dark color */
    --color-secondary: #0f4c75;    /* Secondary blue */
    --color-accent: #3282b8;       /* Links, highlights */
    --color-light: #bbe1fa;        /* Light blue */
    --color-bg: #ffffff;           /* Background */
    --color-text: #2d3436;         /* Body text */
    --color-text-light: #636e72;   /* Secondary text */
    --color-border: #e8ecef;       /* Borders */
}
```

### Current Font

The site uses **Avenir** as specified. It's defined in `styles.css`:

```css
:root {
    --font-serif: 'Avenir', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
    --font-sans: 'Avenir', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
}
```

To change fonts:
1. Open `styles.css`
2. Update the font variables in `:root`
3. If using Google Fonts, add import at top of CSS file

## 🔧 Page Organization

### HTML Files
- **index.html**: Landing page with featured publications
- **research.html**: Publications (55+), grants, PhD students, professional activities
- **teaching.html**: Teaching experience and academic service

### Shared Resources
- **styles.css**: All styles including Avenir font and color scheme
- **script.js**: JavaScript for navigation and interactions
- **img/**: Photos (chris.png, logo.png)

### Navigation Structure
```
Home (index.html)
  ├─ About
  ├─ Featured Publications (5 recent)
  └─ Contact

Research (research.html)
  ├─ Publications (All 55+)
  ├─ Research Grants
  ├─ PhD Supervision
  └─ Professional Activities

Teaching (teaching.html)
  ├─ Qualifications
  ├─ Current Teaching
  ├─ Previous Teaching
  └─ Academic Service
```

## 📊 Content Summary

Your website includes:
- ✅ Complete bio and research description
- ✅ 5 featured publications on landing page
- ✅ 55+ publications organized by year (2025-2014)
- ✅ 7 major research grants + industry grants
- ✅ 6 current PhD students with topics and supervisors
- ✅ Comprehensive professional activities
- ✅ Teaching qualifications (FHEA, AFHEA)
- ✅ Current and past teaching (Bath + Lancaster)
- ✅ Academic service and committee work
- ✅ Contact: chrisclarke@acm.org

## 🆘 Troubleshooting

**Problem: Navigation not working**
- Ensure all files are in the same directory
- Check filenames match exactly (case-sensitive)
- Verify styles.css and script.js are in root

**Problem: Avenir font not showing**
- Avenir is a system font on Mac/iOS
- On Windows/Linux, it falls back to system sans-serif
- This is intentional and works correctly

**Problem: Research page too long**
- This is normal with 55+ publications
- Content is organized by year for easy scanning
- Consider using browser's Find function (Ctrl+F)

**Problem: Changes not appearing on GitHub Pages**
- Wait 2-3 minutes for rebuild
- Check Actions tab for build status
- Hard refresh (Ctrl+Shift+R or Cmd+Shift+R)

## 📱 Mobile Optimization

✅ Responsive navigation with hamburger menu  
✅ Mobile-friendly layouts that stack properly  
✅ Touch-friendly button sizes  
✅ Optimized font sizes for all devices  

## 🔄 Maintenance Best Practices

1. **Update publications** as papers are accepted
2. **Add grants** when funding is awarded
3. **Update PhD students** when students join/graduate
4. **Refresh activities** after conference roles
5. **Test locally** before pushing to GitHub
6. **Backup files** before major changes

## 📧 Quick Reference

| Content | File | Section |
|---------|------|---------|
| Featured papers | index.html | Featured Publications |
| All publications | research.html | Publications |
| Grants | research.html | Research Grants |
| PhD students | research.html | PhD Supervision |
| Professional service | research.html | Professional Activities |
| Teaching | teaching.html | Various sections |
| Contact info | index.html | Contact |
| Colors/fonts | styles.css | :root |

---

**Version**: 2.0 (Multi-page with Research)  
**Last Updated**: February 2025  
**Font**: Avenir  
**Email**: chrisclarke@acm.org  
**Pages**: 3 (Home, Research, Teaching)  
**Publications**: 55+  
**Grants**: 7 major + industry  
**PhD Students**: 6 current
