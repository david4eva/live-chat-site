# GeoContact Platform Website

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Salesforce](https://img.shields.io/badge/Salesforce-00A1E0?style=for-the-badge&logo=salesforce&logoColor=white)

[![Mobile Responsive](https://img.shields.io/badge/Mobile-Responsive-brightgreen)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Responsive/responsive_design_building_blocks)
[![SEO Optimized](https://img.shields.io/badge/SEO-Optimized-success)](#seo-features)
[![Chat Ready](https://img.shields.io/badge/Salesforce%20Chat-Ready-blue)](#salesforce-chat-integration)

A modern, responsive landing page showcasing the Contact Distance Search Lightning Web Component. Built with vanilla HTML, CSS, and JavaScript, featuring integrated Salesforce Chat capabilities and optimized for professional presentation.

## Live Demo

**🌐 [View Live Site](https://your-github-pages-url.github.io/geocontact-website/)**

*Deployed via GitHub Pages with automatic updates*

## Features

### Modern Design System
- **Clean Aesthetics**: Minimalist design with professional color scheme
- **Custom CSS Variables**: Consistent theming throughout the site
- **Smooth Animations**: Fade-in effects and hover transitions
- **Typography**: Inter font family for modern, readable text

### Responsive Architecture
- **Mobile-First Design**: Optimized layouts for all screen sizes
- **Flexible Grid System**: CSS Grid and Flexbox for adaptive layouts
- **Touch-Friendly Interface**: Optimized button sizes and spacing
- **Cross-Browser Compatible**: Tested across major browsers

### Performance Optimized
- **Vanilla JavaScript**: No framework dependencies for fast loading
- **Optimized Assets**: Efficient use of external resources
- **Lazy Loading**: Intersection Observer for performance
- **SEO Ready**: Meta tags and semantic HTML structure

### Salesforce Integration
- **Chat Widget Ready**: Pre-configured container for Salesforce Chat
- **Enterprise Positioning**: Professional presentation for B2B audiences
- **Lead Generation**: Contact forms and call-to-action optimization

## Project Structure

```
geocontact-website/
├── index.html              # Main website file
├── README.md               # This documentation
├── assets/                 # Static assets directory
│   ├── images/            # Screenshots and graphics
│   │   ├── desktop-view.png
│   │   ├── mobile-view.png
│   │   └── demo-preview.png
│   ├── videos/            # Demo videos
│   │   └── component-demo.mp4
│   └── docs/              # Additional documentation
│       └── salesforce-chat-setup.md
├── styles/                # CSS files (if separated)
│   └── main.css
└── scripts/               # JavaScript files (if separated)
    └── main.js
```

## Quick Start

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/geocontact-website.git
   cd geocontact-website
   ```

2. **Open in VS Code**
   ```bash
   code .
   ```

3. **Install Live Server extension** (recommended)
   - Extensions → Search "Live Server" by Ritwick Dey
   - Install the extension

4. **Start development server**
   - Right-click `index.html` → "Open with Live Server"
   - Site opens at `http://localhost:5500`

### Alternative Viewing Methods

#### Option A: VS Code Live Preview
```bash
# Install Live Preview extension by Microsoft
# Right-click index.html → "Show Preview"
```

#### Option B: Simple File Opening
```bash
# Double-click index.html to open in default browser
# No server required for basic functionality
```

## Customization Guide

### Branding Updates

1. **Site Title and Meta**
   ```html
   <title>Your Company - Geospatial Intelligence Platform</title>
   <meta name="description" content="Your custom description">
   ```

2. **Logo and Company Name**
   ```html
   <!-- Update in navigation -->
   <a href="#" class="logo">
       <i class="fas fa-map-marked-alt"></i> YourBrand
   </a>
   ```

3. **Color Scheme**
   ```css
   :root {
       --primary-color: #your-brand-color;
       --secondary-color: #your-secondary-color;
       /* Update other color variables */
   }
   ```

### Content Updates

1. **Hero Section**
   - Update headline and description
   - Modify call-to-action buttons
   - Replace background elements

2. **Features Section**
   - Add/remove feature cards
   - Update icons and descriptions
   - Modify grid layout

3. **Contact Information**
   - Update social media links
   - Add contact details
   - Modify footer content

## Salesforce Chat Integration

### Setup Instructions

1. **Obtain Chat Widget Code**
   - Navigate to Salesforce Setup → Chat Settings
   - Generate embedded chat code
   - Copy the JavaScript snippet

2. **Add to Website**
   ```html
   <!-- Replace the commented section in index.html -->
   <div class="chat-widget">
       <!-- Paste your Salesforce Chat code here -->
       <script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
       <script type='text/javascript'>
           // Your Salesforce Chat configuration
       </script>
   </div>
   ```

3. **Configuration Options**
   ```javascript
   embedded_svc.settings.displayHelpButton = true;
   embedded_svc.settings.language = '';
   embedded_svc.settings.defaultMinimizedText = 'Chat with us';
   embedded_svc.settings.disabledMinimizedText = 'Agent Offline';
   ```

### Chat Widget Styling

The chat widget container includes proper positioning and z-index management:

```css
.chat-widget {
    position: fixed;
    bottom: 2rem;
    right: 2rem;
    z-index: 1001;
}
```

## SEO Features

### Meta Tags
- Open Graph tags for social sharing
- Twitter Card meta tags
- Structured data markup
- Canonical URL specification

### Performance
- Optimized image loading
- Minified CSS and JavaScript
- Efficient font loading strategy
- Compressed assets

### Accessibility
- Semantic HTML structure
- ARIA labels and roles
- Keyboard navigation support
- Screen reader compatibility

## Deployment Options

### GitHub Pages (Recommended)

1. **Enable GitHub Pages**
   ```bash
   # Push code to GitHub repository
   git add .
   git commit -m "Initial website deployment"
   git push origin main
   
   # Go to repository Settings → Pages
   # Select source: Deploy from branch (main)
   ```

2. **Custom Domain** (optional)
   ```bash
   # Add CNAME file with your domain
   echo "your-domain.com" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push origin main
   ```

### Alternative Hosting

#### Netlify
```bash
# Drag and drop project folder to Netlify dashboard
# Automatic deployment from GitHub integration available
```

#### Vercel
```bash
npm i -g vercel
vercel --prod
```

#### Traditional Web Hosting
```bash
# Upload index.html and assets via FTP
# Ensure proper file permissions
```

## Browser Support

| Browser | Desktop | Mobile | Notes |
|---------|---------|--------|-------|
| Chrome  | ✅ Latest | ✅ Latest | Full feature support |
| Firefox | ✅ Latest | ✅ Latest | Full feature support |
| Safari  | ✅ Latest | ✅ Latest | Full feature support |
| Edge    | ✅ Latest | ✅ Latest | Full feature support |
| IE 11   | ⚠️ Limited | ❌ No | Basic layout only |

## Performance Metrics

### Lighthouse Scores (Target)
- **Performance**: 95+
- **Accessibility**: 100
- **Best Practices**: 100
- **SEO**: 100

### Loading Speed
- **First Contentful Paint**: < 1.5s
- **Largest Contentful Paint**: < 2.5s
- **Cumulative Layout Shift**: < 0.1

## Contributing

### Development Workflow

1. **Fork the repository**
2. **Create feature branch**
   ```bash
   git checkout -b feature/improvement-name
   ```
3. **Make changes**
4. **Test across browsers and devices**
5. **Submit pull request**

### Code Standards

- **HTML**: Semantic markup, proper nesting
- **CSS**: BEM methodology, consistent naming
- **JavaScript**: ES6+ features, proper error handling
- **Comments**: Clear documentation for complex sections

### Testing Checklist

- [ ] Responsive design on multiple screen sizes
- [ ] Cross-browser compatibility
- [ ] Accessibility standards compliance
- [ ] Performance optimization
- [ ] SEO meta tags verification
- [ ] Salesforce Chat integration testing

## Roadmap

### Planned Enhancements
- **Interactive Demo**: Embedded component showcase
- **Video Integration**: Auto-playing demo videos
- **Analytics Integration**: Google Analytics/Salesforce tracking
- **Multi-language Support**: Internationalization features
- **Progressive Web App**: Offline functionality
- **Advanced Animations**: More sophisticated transitions

### Content Additions
- **Case Studies**: Customer success stories
- **Technical Documentation**: Implementation guides
- **API Documentation**: Integration specifications
- **Blog Section**: Industry insights and updates

## Support and Resources

### Documentation
- [Salesforce Chat Setup Guide](assets/docs/salesforce-chat-setup.md)
- [Customization Examples](https://github.com/yourusername/geocontact-website/wiki)
- [Deployment Guide](https://pages.github.com/)

### Community
- [GitHub Issues](https://github.com/yourusername/geocontact-website/issues)
- [Discussions](https://github.com/yourusername/geocontact-website/discussions)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Salesforce Lightning Design System** for design inspiration
- **Font Awesome** for iconography
- **Google Fonts** for typography
- **Modern CSS techniques** from web development community

---

**⭐ Star this repository if it helped showcase your Salesforce projects!**
