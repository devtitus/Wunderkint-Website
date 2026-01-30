# 🚀 Wunderkint Creative Agency Website

A modern, responsive website that showcases the creative solutions offered by Wunderkint Agency. Built with HTML5, CSS3, and vanilla JavaScript, it features interactive animations, a dynamic portfolio gallery, and client testimonials. The website is designed to provide an engaging user experience while effectively communicating the agency's services and portfolio.

## ✨ Features

- 🎨 **Animated hero and service sections** with smooth transitions and interactive elements
- 📹 **Portfolio gallery** with video previews, filtering options, and hover effects
- 🗣️ **Client testimonial carousel** with smooth scrolling and responsive design
- 💰 **Flexible pricing plans** with comparison table and interactive elements
- 📱 **Mobile-first responsive design** that adapts to all screen sizes
- 🎬 **Video integration** with autoplay and hover-to-play functionality
- 🎨 **Custom animations** using CSS3 transitions and JavaScript
- 📊 **Interactive elements** including hover states and smooth scrolling
- 🌐 **SEO optimized** with proper meta tags and structured data
- 🔧 **Smooth scrolling** implementation using Lenis library
- 🎵 **Audio integration** with Howler.js for interactive sound effects
- 📈 **Analytics integration** with Google Tag Manager
- 🎨 **Custom branding** with unique color schemes and typography
- 📱 **Cross-browser compatibility** ensuring consistent experience
- ⚡ **Optimized performance** with lazy loading and asset optimization

## 🛠️ Tech Stack

### Core Technologies
- **HTML5** – Semantic markup and structure
- **CSS3** – Custom styles, animations, and responsive layout
- **JavaScript** – Interactive components and filtering logic

### Frameworks & Libraries
- **Webflow CSS Framework** – Pre-built components and animations
- **Lenis** – Smooth scrolling implementation
- **Howler.js** – Audio management and playback
- **Google Tag Manager** – Analytics and tracking

### Development Tools
- **Netlify** – Static site hosting and continuous deployment
- **Git** – Version control and collaboration
- **Visual Studio Code** – Development environment

### Assets & Media
- **SVG Icons** – Scalable vector graphics for UI elements
- **WebP Images** – Optimized image format for web
- **Video Files** – Portfolio showcase and background videos
- **Custom Fonts** – Typography and branding elements

## 📁 Folder Structure

```
wunderkint-website/
├── .gitignore                 # Git ignore rules
├── .htaccess                  # Apache server configuration
├── index.html                 # Main entry point and HTML structure
├── netlify.toml               # Netlify deployment configuration
├── README.md                  # This file
├── robots.txt                 # Search engine instructions
├── sitemap.xml                # Website sitemap
├── css/                       # Stylesheets directory
│   ├── normalize.css          # CSS reset and normalization
│   ├── webflow.css            # Webflow framework styles
│   ├── wunderkint-new-site.webflow.css  # Main custom styles
│   └── insta-grid.css         # Instagram grid styles
├── favicon/                   # Favicon assets
│   ├── android-chrome-192x192.png
│   ├── android-chrome-512x512.png
│   ├── apple-touch-icon.png
│   ├── favicon-16x16.png
│   ├── favicon-32x32.png
│   ├── favicon.ico
│   └── site.webmanifest
├── fonts/                     # Custom font files
│   └── Cherie_DEMO.ttf        # Primary font
├── images/                    # Image assets
│   ├── hero/                  # Hero section images
│   ├── portfolio/             # Portfolio project images
│   ├── testimonials/          # Client testimonial images
│   ├── branding/              # Branding solution images
│   ├── web-solutions/         # Web solutions images
│   ├── media-solutions/       # Media solutions images
│   ├── pricing/               # Pricing plan images
│   ├── icons/                 # UI icons and symbols
│   └── backgrounds/           # Background images and patterns
├── js/                        # JavaScript files
│   ├── webflow.js             # Webflow interactions
│   ├── lenis.js               # Smooth scrolling
│   ├── howler.js              # Audio management
│   └── custom.js              # Custom JavaScript functionality
└── pages/                     # Additional HTML pages
    ├── about-us.html          # About page
    ├── branding-solutions.html # Branding solutions page
    ├── web-solutions.html     # Web solutions page
    ├── media-solutions.html   # Media solutions page
    └── contact.html           # Contact page
```

## ⚙️ Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Edge, Safari)
- Code editor (Visual Studio Code recommended)
- Git for version control

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/devtitus/Wunderkint-Website.git
   cd wunderkint-website
   ```

2. **Install dependencies** (if any)
   ```bash
   # No external dependencies required for this static site
   ```

3. **Open the website**
   - Option 1: Open `index.html` directly in your browser
   - Option 2: Use a local development server
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js
     npx serve .
     
     # Using Netlify CLI (if available)
     netlify dev
     ```

4. **View the website**
   - Navigate to `http://localhost:8000` in your browser
   - The website should load with all features and animations

### Development

1. **Make changes to HTML/CSS/JS files**
   - Edit `index.html` for structure changes
   - Modify CSS files in the `css/` directory
   - Update JavaScript in the `js/` directory

2. **Test changes**
   - Refresh your browser to see updates
   - Test on different screen sizes using browser dev tools
   - Check functionality across different browsers

3. **Deploy changes**
   - Commit changes to Git
   - Push to the repository
   - Netlify will automatically deploy the updated site

## 🚀 Deployment

### Netlify Configuration

The website is configured for automatic deployment through Netlify:

1. **Netlify.toml Configuration**
   - Build command: None (static site)
   - Publish directory: Root directory
   - Production branch: main

2. **Deployment Process**
   - Push changes to the main branch
   - Netlify automatically builds and deploys
   - Website updates are live within minutes

3. **Custom Domain**
   - Configure custom domain in Netlify settings
   - SSL certificate automatically provisioned
   - CDN distribution for global performance

### Environment Variables

For local development, you may need to configure environment variables:

```bash
# Google Analytics (if applicable)
GOOGLE_ANALYTICS_ID=UA-XXXXXXXXX-X

# Google Tag Manager (if applicable)
GTM_CONTAINER_ID=GTM-XXXXXXX
```

## 🤝 Contributing

We welcome contributions to the Wunderkint Creative Agency website! Please follow these guidelines:

### Getting Started

1. **Fork the repository**
   - Click the "Fork" button on the GitHub repository
   - Clone your forked repository

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**
   - Follow the existing code style
   - Test your changes thoroughly
   - Update documentation if necessary

4. **Submit a pull request**
   - Push your changes to your fork
   - Create a pull request to the main repository
   - Describe your changes and why they're beneficial

### Code Style

- Use semantic HTML5 elements
- Follow BEM methodology for CSS class names
- Use ES6+ JavaScript features
- Include proper comments and documentation
- Maintain consistent indentation and formatting

### Testing

- Test on multiple browsers (Chrome, Firefox, Safari, Edge)
- Check responsive design on different screen sizes
- Verify all interactive elements work correctly
- Test performance and loading times

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Attribution

- Webflow CSS Framework - https://webflow.com
- Lenis Smooth Scrolling - https://github.com/studio-freight/lenis
- Howler.js Audio Library - https://github.com/goldfire/howler.js
- Google Fonts - https://fonts.google.com

## 🔗 Additional Resources

- **Project Documentation**: [PROJECT.md](PROJECT.md)
- **Setup Guide**: [SETUP-GUIDE.md](SETUP-GUIDE.md)
- **GitHub Repository**: https://github.com/devtitus/Wunderkint-Website
- **Live Website**: https://www.wunderkint.com

## 📧 Contact

For questions, support, or collaboration opportunities, please contact:

- **Email**: info@wunderkint.com
- **Website**: https://www.wunderkint.com
- **Instagram**: https://www.instagram.com/wunderkint/
- **LinkedIn**: https://in.linkedin.com/company/wunderkint
- **Facebook**: https://www.facebook.com/p/Wunderkint-Creative-Private-Limited-61558976992384/
- **Behance**: https://www.behance.net/wunderkcreativ

---

*Last updated: January 2026*