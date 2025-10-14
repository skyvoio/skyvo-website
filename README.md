# Skyvo Website

A modern, professional website for Skyvo - a Drones • Robotics • AI consulting firm based in the Greater Toronto Area.

## Overview

This website showcases Skyvo's capabilities in aerial mapping, autonomous robotics, and intelligent automation. It's built with clean HTML, CSS, and JavaScript, optimized for performance and fully compatible with GitHub Pages.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations and transitions
- **SEO Optimized**: Proper meta tags, semantic HTML, and clean URL structure
- **Accessible**: High contrast ratios (≥4.5:1) and descriptive alt text
- **Fast Loading**: Minimal dependencies, optimized assets
- **Interactive Elements**: Smooth scrolling, scroll-reveal animations, hover effects

## Sections

1. **Hero** - Three headline options with CTAs
2. **Trust Strip** - Credibility statement
3. **Three Pillars** - Drones, Robotics, and AI solutions
4. **Use Cases** - Six industry-specific applications
5. **Case Studies** - Three anonymized success stories with metrics
6. **Process** - Four-step methodology (Discover → Pilot → Deploy → Scale)
7. **Tech Stack** - Technology ribbon showcasing tools and platforms
8. **Compliance & Safety** - Transport Canada RPAS certification details
9. **FAQ** - Six frequently asked questions
10. **Contact** - Contact form with company information

## Deployment to GitHub Pages

### Option 1: Using GitHub Web Interface

1. Create a new repository on GitHub (e.g., `skyvo-website`)
2. Upload all files from this directory to the repository:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`
3. Go to repository Settings → Pages
4. Under "Source", select "Deploy from a branch"
5. Select the `main` branch and `/ (root)` folder
6. Click "Save"
7. Your site will be published at `https://[username].github.io/skyvo-website/`

### Option 2: Using Git Command Line

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Skyvo website"

# Add remote repository (replace with your repository URL)
git remote add origin https://github.com/[username]/skyvo-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then follow steps 3-7 from Option 1.

### Option 3: Using Custom Domain

If you want to use the `skyvo.io` domain:

1. Follow the deployment steps above
2. In your repository, go to Settings → Pages
3. Under "Custom domain", enter `skyvo.io`
4. Click "Save"
5. In your domain registrar (where you bought skyvo.io), add these DNS records:
   - Type: `A`, Name: `@`, Value: `185.199.108.153`
   - Type: `A`, Name: `@`, Value: `185.199.109.153`
   - Type: `A`, Name: `@`, Value: `185.199.110.153`
   - Type: `A`, Name: `@`, Value: `185.199.111.153`
   - Type: `CNAME`, Name: `www`, Value: `[username].github.io`
6. Wait for DNS propagation (can take up to 24 hours)
7. Enable "Enforce HTTPS" in GitHub Pages settings

## File Structure

```
skyvo-website/
├── index.html          # Main HTML file with all content
├── styles.css          # Complete stylesheet with responsive design
├── script.js           # JavaScript for interactivity and animations
└── README.md           # This file
```

## Customization

### Updating Contact Information

The contact information is already set to:
- **Email**: hello@skyvo.io
- **Phone**: 416-805-8408
- **Website**: skyvo.io

To update these, search and replace in `index.html`:
- Email: Find `hello@skyvo.io` and replace
- Phone: Find `416-805-8408` and replace
- Website: Find `skyvo.io` and replace

### Changing Colors

The color palette is defined in `styles.css` using CSS variables:

```css
:root {
    --color-ink: #0F172A;        /* Dark blue/black */
    --color-cobalt: #0EA5E9;     /* Primary blue */
    --color-teal: #14B8A6;       /* Accent teal */
    --color-light-gray: #E2E8F0; /* Light gray */
    --color-white: #FFFFFF;      /* White */
    --color-signal: #F59E0B;     /* Orange accent */
}
```

### Adding Images

To replace the SVG placeholders with real images:

1. Add your images to an `images/` folder
2. In `index.html`, replace the SVG elements with:
   ```html
   <img src="images/your-image.jpg" alt="Descriptive alt text">
   ```

### Modifying Content

All content is in `index.html`. The structure is semantic and well-commented. Simply find the section you want to modify and update the text.

## Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- No external dependencies (except Google Fonts)
- Minimal JavaScript
- Optimized CSS with no bloat
- Fast loading times

## Contact Form

The contact form currently shows an alert message. To make it functional:

1. Use a form service like Formspree, Netlify Forms, or Google Forms
2. Or add a backend API endpoint
3. Update the form submission handler in `script.js`

Example with Formspree:

```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

## License

Copyright © 2025 Skyvo. All rights reserved.

## Support

For questions or support, contact:
- Email: hello@skyvo.io
- Phone: 416-805-8408
- Website: https://skyvo.io

