# Portfolio Website - Setup Instructions

## 📋 Overview
A modern, responsive portfolio website built with HTML, CSS, and JavaScript. Features include smooth animations, typing effects, contact form, and mobile-friendly design.

## 🚀 Quick Start

### Option 1: Simple Setup
1. Place all three files (`index.html`, `style.css`, `script.js`) in the same folder
2. Open `index.html` in your web browser
3. That's it! Your portfolio is ready to view locally

### Option 2: Web Hosting
Upload all three files to your web hosting service:
- **GitHub Pages**: Push to a GitHub repo and enable Pages
- **Netlify**: Drag and drop all files
- **Vercel**: Connect your GitHub repo or upload files
- **Traditional hosting**: Upload via FTP to your server

## 📁 File Structure
```
portfolio/
│
├── index.html      # Main HTML file
├── style.css       # All styles and animations
└── script.js       # Interactive functionality
```

## 🎨 Customization Guide

### 1. Personal Information
**In `index.html`:**
- Line 15: Update page title
- Lines 52-54: Update hero greeting and title
- Lines 80-86: Add your email, phone, location
- Lines 342-350: Update contact information
- Lines 373-377: Update social media links

### 2. Profile Image
**To add your photo:**
Replace the placeholder section (lines 87-93) with:
```html
<div class="image-wrapper">
    <img src="your-photo.jpg" alt="Your Name" style="width: 100%; height: 450px; object-fit: cover; border-radius: 50%;">
</div>
```

### 3. Projects
**In `index.html` (lines 232-338):**
- Update project names, descriptions, and tech stacks
- Add/remove project cards as needed
- Update GitHub links

### 4. Skills
**In `index.html` (lines 160-229):**
- Modify skill names and proficiency levels
- Add new skills by copying a skill-card block

### 5. Experience & Education
**In `index.html`:**
- Experience: Lines 195-231
- Education: Lines 122-141
- Update dates, companies, and descriptions

### 6. Color Scheme
**In `style.css` (lines 1-18):**
```css
--primary-color: #6366f1;    /* Main brand color */
--secondary-color: #8b5cf6;  /* Accent color */
--accent-color: #ec4899;     /* Highlight color */
```

### 7. Typing Effect
**In `script.js` (lines 1-5):**
```javascript
const textArray = [
    'Your Title 1',
    'Your Title 2',
    'Your Title 3'
];
```

## 📧 Contact Form Setup

### Current Status
The contact form has client-side validation but needs backend integration.

### Integration Options:

#### Option 1: Formspree (Easiest - No Code)
1. Sign up at https://formspree.io
2. Update form action in `index.html`:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

#### Option 2: EmailJS (Free, No Backend)
1. Sign up at https://www.emailjs.com
2. Add EmailJS script to `index.html`
3. Update `script.js` contact form function

#### Option 3: Your Own Backend
Uncomment lines 171-183 in `script.js` and connect to your API endpoint.

#### Option 4: Supabase (Like Your Flask App)
1. Keep your existing Supabase setup
2. Add Supabase JavaScript client
3. Update the form submission in `script.js`

## 📥 CV/Resume Download

**To enable CV download:**
1. Add your CV file (PDF format recommended) to the same folder
2. Update line 219 in `script.js`:
```javascript
window.location.href = 'your-cv.pdf';
```

## 🎯 Features

✅ **Responsive Design** - Works on all devices
✅ **Smooth Animations** - Fade-ins, typing effect, progress bars
✅ **Interactive Navigation** - Sticky navbar with active link highlighting
✅ **Contact Form** - With validation (ready for backend)
✅ **Project Showcase** - Beautiful card layout with hover effects
✅ **Skills Display** - Animated progress bars
✅ **Timeline Layout** - Professional experience section
✅ **Social Links** - GitHub, LinkedIn, Email, Twitter
✅ **Scroll to Top** - Smooth scroll button
✅ **Mobile Menu** - Hamburger navigation for mobile devices

## 🌐 Browser Compatibility
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

## 🎨 Dependencies
- Font Awesome 6.4.0 (loaded via CDN)
- Inter font family (system fonts fallback)

No npm packages or build tools required!

## 📱 Mobile Optimization
- Responsive breakpoints: 968px, 768px, 480px
- Touch-friendly navigation
- Optimized images and animations
- Mobile-first approach

## 🔧 Troubleshooting

**Icons not showing?**
- Check internet connection (Font Awesome is loaded from CDN)

**Animations not working?**
- Ensure JavaScript is enabled in browser
- Check browser console for errors

**Form not submitting?**
- Form requires backend integration (see Contact Form Setup)

## 🚀 Performance Tips
1. Compress images before uploading
2. Use WebP format for better compression
3. Minify CSS and JS for production
4. Enable caching on your server

## 📄 License
Free to use and modify for personal and commercial projects.

## 💡 Next Steps
1. Update all personal information
2. Add your profile photo
3. Update projects and skills
4. Set up contact form backend
5. Add your CV/resume file
6. Customize colors to match your brand
7. Deploy to your hosting service

## 🤝 Support
If you need help customizing or have questions:
- Check the comments in the code
- Review this README
- Test changes locally before deploying

---

**Built with ❤️ - Good luck with your portfolio!**
