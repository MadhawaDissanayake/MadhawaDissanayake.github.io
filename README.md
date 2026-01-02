# Portfolio Website

A modern, professional portfolio website showcasing Machine Learning projects, Algorithmic Trading strategies, and Wildlife Photography.

## Live Site

Visit the live site at: [https://madhawadissanayake.github.io/](https://madhawadissanayake.github.io/)

## Features

### Design & UI/UX
- Modern, responsive design using Tailwind CSS
- Smooth scroll navigation with active link highlighting
- Gradient backgrounds and animations
- Mobile-first approach with hamburger menu
- Professional color scheme (Indigo/Purple/Pink gradients)
- Fully accessible with keyboard navigation support

### Sections

1. **Hero Section**
   - Full-height landing page with gradient background
   - Professional introduction and tagline
   - Call-to-action buttons
   - Animated scroll indicator

2. **About Section**
   - Two-column responsive layout
   - Skills showcase with animated progress bars
   - Technology stack badges
   - Profile image placeholder

3. **Machine Learning Projects**
   - Grid layout with 6 project cards
   - Placeholder charts for model metrics
   - Project descriptions and tech tags
   - GitHub and "View Details" buttons

4. **Photography Gallery**
   - Responsive grid layout with 9 images
   - Category filtering (All, Wildlife, Landscape, Macro)
   - Lightbox functionality for full-size viewing
   - Keyboard navigation support (← → arrows, ESC to close)
   - Smooth hover effects

5. **Trading Dashboard**
   - Financial dashboard aesthetic
   - Statistics cards (Returns, Win Rate, Sharpe Ratio, Drawdown)
   - Performance chart visualization
   - Recent trades table
   - Risk metrics with progress indicators

6. **Contact Section**
   - Functional contact form with validation
   - Social media links (GitHub, LinkedIn, Twitter, Instagram)
   - Contact information cards
   - Success/error message display

7. **Footer**
   - Quick links to all sections
   - Technology list
   - Social media icons
   - Copyright information

### Interactive Features

- **Mobile Menu**: Fully functional hamburger menu for mobile devices
- **Smooth Scrolling**: Smooth scroll to sections when clicking navigation links
- **Scroll Animations**: Fade-in effects as elements come into view
- **Navbar Effects**: Shadow and styling changes on scroll
- **Gallery Filtering**: Dynamic filtering of photography by category
- **Lightbox**: Full-screen image viewer with navigation
- **Form Validation**: Client-side email and required field validation
- **Lazy Loading**: Optimized image loading for better performance

## Technology Stack

- **HTML5**: Semantic markup
- **CSS3**: Custom styles and animations
- **Tailwind CSS**: Utility-first CSS framework (via CDN)
- **Vanilla JavaScript**: No frameworks, pure JS for maximum performance
- **Font Awesome**: Icon library
- **Google Fonts**: Inter font family

## File Structure

```
/
├── index.html              # Main HTML file with all sections
├── css/
│   └── custom.css          # Custom styles and animations
├── js/
│   └── main.js             # All JavaScript functionality
├── images/
│   └── .gitkeep            # Placeholder for images folder
└── README.md               # This file
```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/madhawadissanayake/madhawadissanayake.github.io.git
cd madhawadissanayake.github.io
```

### 2. Customize Your Content

#### Update Personal Information

In `index.html`, search for these placeholders and replace with your own content:

- **Name**: Replace "Madhawa Dissanayake" with your name
- **Email**: Update `your.email@example.com` in the contact section
- **Location**: Update "Your City, Country"
- **Social Links**: Replace `#` with your actual social media URLs

#### Add Your Projects

1. Find the Projects section in `index.html` (starting at line ~400)
2. Update the 6 project cards with your actual projects:
   - Change project titles and descriptions
   - Update technology tags
   - Add GitHub repository links
   - Replace placeholder images with your project screenshots

#### Add Your Photography

1. Add your images to the `images/` folder
2. Update image sources in the Photography section
3. Organize by categories (wildlife, landscape, macro)
4. The lightbox will automatically work with your images

#### Update Trading Dashboard

1. Replace placeholder statistics with your actual data
2. Update the performance chart values
3. Modify the recent trades table
4. Adjust risk metrics

#### Customize About Section

1. Rewrite the bio paragraphs
2. Adjust skill percentages
3. Update technology stack badges
4. Replace profile image placeholder

### 3. Add Your Images

Place your images in the `images/` folder:

```
images/
├── profile.jpg              # Your profile photo
├── projects/
│   ├── project1.png
│   ├── project2.png
│   └── ...
└── photography/
    ├── wildlife1.jpg
    ├── landscape1.jpg
    └── ...
```

Then update image sources in `index.html`:

```html
<!-- Example -->
<img src="images/profile.jpg" alt="Your Name">
<img src="images/projects/project1.png" alt="Project Name">
```

### 4. Deploy to GitHub Pages

1. Push your changes to GitHub:
   ```bash
   git add .
   git commit -m "Initial portfolio setup"
   git push origin main
   ```

2. Enable GitHub Pages:
   - Go to your repository settings
   - Navigate to "Pages" section
   - Select source: `main` branch
   - Click "Save"

3. Your site will be live at: `https://yourusername.github.io/`

## Customization Guide

### Change Color Scheme

The site uses a Tailwind CSS configuration with custom colors. To change colors, update the `tailwind.config` in `index.html`:

```javascript
tailwind.config = {
    theme: {
        extend: {
            colors: {
                primary: '#6366f1',    // Change this
                secondary: '#8b5cf6',  // Change this
                accent: '#ec4899',     // Change this
            }
        }
    }
}
```

### Modify Fonts

To change fonts, update the Google Fonts link in `index.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
```

Then update the font family in `tailwind.config`:

```javascript
fontFamily: {
    sans: ['YourFont', 'sans-serif'],
}
```

### Add More Sections

To add a new section:

1. Add the section HTML before the footer
2. Add a navigation link in the navbar
3. Add scroll animations if desired
4. Update the footer quick links

## Form Integration

The contact form currently validates on the client-side only. To receive actual emails, integrate with:

### Option 1: Formspree (Recommended)

1. Sign up at [Formspree](https://formspree.io/)
2. Update the form in `index.html`:
   ```html
   <form id="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
3. Remove the `preventDefault()` in `main.js` form handler

### Option 2: EmailJS

1. Sign up at [EmailJS](https://www.emailjs.com/)
2. Follow their integration guide
3. Add EmailJS SDK and update the form handler in `main.js`

### Option 3: Custom Backend

Create your own backend API to handle form submissions.

## Performance Optimization

The website is already optimized with:

- Lazy loading for images
- Minimal external dependencies
- CSS/JS minification ready
- Efficient animations using CSS transforms
- Intersection Observer for scroll animations

### Further Optimizations

1. **Image Compression**: Use tools like TinyPNG or ImageOptim
2. **CDN**: Consider self-hosting Tailwind CSS for production
3. **Minification**: Minify HTML, CSS, and JS files
4. **Caching**: Add service worker for offline support

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Accessibility

The website includes:

- Semantic HTML5 elements
- ARIA labels where appropriate
- Keyboard navigation support
- Focus indicators for keyboard users
- Alt text placeholders for images
- Skip to content link
- Screen reader friendly structure

## SEO

Included meta tags for SEO:

- Title and description
- Keywords
- Author
- Open Graph tags (add for social media sharing)

### Add Open Graph Tags

Add these to `<head>` for better social media sharing:

```html
<meta property="og:title" content="Your Name - Portfolio">
<meta property="og:description" content="Your description">
<meta property="og:image" content="https://yoursite.com/images/og-image.jpg">
<meta property="og:url" content="https://yoursite.com">
<meta name="twitter:card" content="summary_large_image">
```

## Easter Eggs

The website includes a Konami Code easter egg! Try typing: ↑ ↑ ↓ ↓ ← → ← → B A

## Future Enhancements

Consider adding:

- [ ] Dark mode toggle
- [ ] Blog section
- [ ] Resume/CV download
- [ ] Project detail pages
- [ ] Animations with GSAP or Framer Motion
- [ ] Progressive Web App (PWA) features
- [ ] Multi-language support
- [ ] Analytics integration (Google Analytics, Plausible)
- [ ] Live chat widget

## License

MIT License - Feel free to use this template for your own portfolio!

## Support

If you have questions or need help customizing:

1. Check this README first
2. Review the code comments in the files
3. Open an issue on GitHub
4. Contact via the contact form

## Credits

- Design & Development: Madhawa Dissanayake
- Built with Tailwind CSS
- Icons by Font Awesome
- Fonts by Google Fonts
- Placeholder images from Unsplash

---

Made with ❤️ using HTML, CSS, and JavaScript
