# Wunderkint Creative Agency Website - Setup Guide

## 📋 Table of Contents

1. [Prerequisites](#prerequisites)
2. [Quick Start](#quick-start)
3. [Development Environment Setup](#development-environment-setup)
4. [Testing Procedures](#testing-procedures)
5. [Troubleshooting](#troubleshooting)
6. [Deployment](#deployment)
7. [Best Practices](#best-practices)

---

## 🚀 Prerequisites

### System Requirements
- **Operating System**: Windows 10/11, macOS 10.15+, Linux (Ubuntu 18.04+)
- **RAM**: Minimum 4GB (8GB recommended)
- **Storage**: 500MB free space
- **Browser**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+

### Software Requirements
- **Code Editor**: Visual Studio Code (recommended) or any preferred editor
- **Git**: Version control system
- **Node.js**: JavaScript runtime (optional, for development tools)
- **Python**: For local development server (optional)
- **Netlify CLI**: For deployment and local testing (optional)

### Browser Extensions
- **Live Server**: For live reloading during development
- **Web Developer**: For debugging and testing
- **Lighthouse**: For performance testing

---

## ⚡ Quick Start

### Method 1: Direct File Opening (Recommended for beginners)

1. **Download the project**
   ```bash
   git clone https://github.com/devtitus/Wunderkint-Website.git
   cd wunderkint-website
   ```

2. **Open in browser**
   - Navigate to the project folder
   - Double-click `index.html` to open in default browser
   - The website should load immediately

### Method 2: Local Development Server

1. **Using Python (built-in)**
   ```bash
   # Navigate to project directory
   cd wunderkint-website
   
   # Start Python server
   python -m http.server 8000
   
   # Or for Python 3
   python3 -m http.server 8000
   ```

2. **Using Node.js**
   ```bash
   # Install serve package globally
   npm install -g serve
   
   # Start development server
   serve .
   ```

3. **Access the website**
   - Open browser and navigate to `http://localhost:8000`
   - The website should load with all features

### Method 3: Netlify CLI (For deployment testing)

1. **Install Netlify CLI**
   ```bash
   npm install -g netlify-cli
   ```

2. **Start Netlify development server**
   ```bash
   netlify dev
   ```

3. **Access the website**
   - Open browser and navigate to `http://localhost:8888`
   - The website should load with Netlify configuration

---

## 🛠️ Development Environment Setup

### 1. Code Editor Setup

#### Visual Studio Code Configuration
1. **Install VS Code Extensions**
   - Live Server by Ritwick Dey
   - Prettier - Code formatter
   - HTMLHint
   - CSSLint
   - JavaScript (ES6) code snippets

2. **Settings Configuration**
   ```json
   {
     "editor.formatOnSave": true,
     "editor.tabSize": 2,
     "editor.detectIndentation": false,
     "files.eol": "\n",
     "prettier.tabWidth": 2,
     "prettier.useTabs": false
   }
   ```

3. **Workspace Settings**
   - Create `.vscode/settings.json` with project-specific settings
   - Configure file associations and formatting rules

### 2. Git Configuration

#### Initial Setup
```bash
# Configure Git username and email
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Verify configuration
git config --global --list
```

#### Repository Setup
```bash
# Initialize Git repository
git init

# Add remote repository
git remote add origin https://github.com/devtitus/Wunderkint-Website.git

# Verify remote
git remote -v
```

### 3. Development Tools Installation

#### Node.js Setup
```bash
# Install Node.js (version 16 or higher)
# Download from https://nodejs.org/

# Verify installation
node --version
npm --version
```

#### Package Installation
```bash
# Install development dependencies
npm install --save-dev prettier eslint htmlhint

# Install build tools (if needed)
npm install --save-dev parcel-bundler webpack
```

---

## 🧪 Testing Procedures

### 1. Browser Testing

#### Manual Testing Steps
1. **Open website in different browsers**
   - Chrome
   - Firefox
   - Safari
   - Edge

2. **Test responsive design**
   - Use browser developer tools
   - Test on different screen sizes
   - Check mobile responsiveness

3. **Verify functionality**
   - Navigation menu
   - Portfolio filtering
   - Video playback
   - Form submissions
   - Smooth scrolling

### 2. Performance Testing

#### Lighthouse Testing
1. **Open Chrome DevTools**
   - Press F12 or right-click and select "Inspect"
   - Go to "Lighthouse" tab

2. **Run performance tests**
   - Select categories: Performance, Accessibility, Best Practices, SEO
   - Click "Generate report"
   - Review results and recommendations

#### Performance Metrics to Check
- **First Contentful Paint**: < 1.5 seconds
- **Largest Contentful Paint**: < 2.5 seconds
- **Time to Interactive**: < 3.5 seconds
- **Cumulative Layout Shift**: < 0.1

### 3. Cross-browser Compatibility Testing

#### Test Matrix
| Browser | Version | OS | Status |
|---------|---------|----|--------|
| Chrome | 90+ | Windows/macOS/Linux | ✅ |
| Firefox | 88+ | Windows/macOS/Linux | ✅ |
| Safari | 14+ | macOS/iOS | ✅ |
| Edge | 90+ | Windows | ✅ |

#### Testing Checklist
- [ ] All interactive elements work
- [ ] Animations play smoothly
- [ ] Responsive design adapts correctly
- [ ] Forms submit properly
- [ ] Videos play without issues
- [ ] Navigation works correctly

---

## 🔧 Troubleshooting

### Common Issues and Solutions

#### Issue 1: Website doesn't load properly
**Symptoms**: Blank page or error messages
**Solutions**:
- Check browser console for errors
- Verify all files are present in correct directories
- Ensure internet connection for external resources
- Try clearing browser cache

#### Issue 2: Animations not working
**Symptoms**: Static elements instead of animated ones
**Solutions**:
- Check JavaScript console for errors
- Verify CSS files are loading correctly
- Ensure Webflow animations are enabled
- Check for conflicting CSS rules

#### Issue 3: Portfolio filtering not working
**Symptoms**: Filter buttons don't respond
**Solutions**:
- Check JavaScript console for errors
- Verify portfolio data structure
- Ensure event listeners are attached
- Check for JavaScript conflicts

#### Issue 4: Videos not playing
**Symptoms**: Video elements show but don't play
**Solutions**:
- Check video file paths
- Verify video formats are supported
- Check browser autoplay policies
- Ensure proper video element attributes

#### Issue 5: Responsive design issues
**Symptoms**: Layout breaks on certain screen sizes
**Solutions**:
- Check CSS media queries
- Verify viewport meta tag
- Test on actual devices if possible
- Use browser developer tools for debugging

### Advanced Troubleshooting

#### Network Issues
```bash
# Check network connectivity
ping google.com

# Check DNS resolution
nslookup google.com

# Check port availability
netstat -an | findstr :8000
```

#### File Permission Issues
```bash
# Check file permissions
ls -la

# Fix permission issues
chmod 644 index.html
chmod 755 css/
chmod 755 js/
```

#### Git Issues
```bash
# Check Git status
git status

# Resolve merge conflicts
git merge --abort
git pull origin main
```

---

## 🚀 Deployment

### 1. Netlify Deployment

#### Prerequisites
- Netlify account
- GitHub repository connected to Netlify
- Domain configured (optional)

#### Deployment Steps
1. **Connect repository to Netlify**
   - Log in to Netlify
   - Click "New site from Git"
   - Select your repository
   - Configure build settings

2. **Configure build settings**
   - Build command: Leave empty (static site)
   - Publish directory: Root directory
   - Production branch: main

3. **Deploy site**
   - Push changes to main branch
   - Netlify automatically builds and deploys
   - Monitor deployment status in Netlify dashboard

#### Custom Domain Setup
1. **Add custom domain**
   - Go to Site settings → Domain management
   - Click "Add custom domain"
   - Enter your domain name
   - Follow DNS configuration instructions

2. **SSL Certificate**
   - Netlify automatically provisions SSL
   - Verify HTTPS is working
   - Test with SSL checker tools

### 2. Manual Deployment

#### FTP Deployment
1. **Connect to FTP server**
   ```bash
   ftp your-server.com
   username: your-username
   password: your-password
   ```

2. **Upload files**
   ```bash
   # Navigate to web root
   cd /var/www/html
   
   # Upload files
   put index.html
   put -r css/
   put -r js/
   put -r images/
   ```

#### Git-based Deployment
```bash
# Add all changes
git add .

# Commit changes
git commit -m "Deploy updates"

# Push to remote
git push origin main
```

---

## 📚 Best Practices

### 1. Code Quality

#### HTML Best Practices
- Use semantic HTML5 elements
- Include proper meta tags
- Add alt attributes to images
- Use proper heading hierarchy
- Validate HTML with W3C validator

#### CSS Best Practices
- Follow BEM methodology
- Use CSS custom properties for variables
- Implement mobile-first responsive design
- Optimize CSS for performance
- Use CSS Grid and Flexbox appropriately

#### JavaScript Best Practices
- Use ES6+ features
- Implement proper error handling
- Use const and let instead of var
- Write modular code
- Add comments for complex logic

### 2. Performance Optimization

#### Image Optimization
- Use WebP format for better compression
- Implement lazy loading for images
- Optimize image sizes for different screen sizes
- Use responsive images with srcset

#### Code Optimization
- Minify CSS and JavaScript files
- Remove unused code and dependencies
- Optimize critical rendering path
- Implement caching strategies

#### Network Optimization
- Use CDN for static assets
- Implement Gzip compression
- Optimize HTTP requests
- Use browser caching

### 3. Security Best Practices

#### Content Security Policy
- Implement proper CSP headers
- Use HTTPS for all resources
- Validate user inputs
- Sanitize data before display

#### Access Control
- Use proper authentication mechanisms
- Implement rate limiting
- Monitor for suspicious activities
- Keep dependencies updated

### 4. Maintenance

#### Regular Updates
- Update dependencies regularly
- Monitor for security vulnerabilities
- Test after updates
- Backup important data

#### Monitoring
- Set up error tracking
- Monitor performance metrics
- Track user behavior
- Analyze traffic patterns

---

## 📋 Checklist Before Launch

### Technical Checklist
- [ ] All pages load correctly
- [ ] Responsive design works on all devices
- [ ] Cross-browser compatibility tested
- [ ] Performance optimized
- [ ] SEO elements implemented
- [ ] Security measures in place
- [ ] Error handling implemented
- [ ] Analytics configured

### Content Checklist
- [ ] All text proofread
- [ ] Images optimized
- [ ] Videos tested
- [ ] Links verified
- [ ] Contact forms working
- [ ] Social media links correct

### Legal Checklist
- [ ] Privacy policy included
- [ ] Terms of service available
- [ ] Cookie consent implemented
- [ ] Copyright notices added
- [ ] License information provided

---

## 📞 Support and Resources

### Documentation
- [README.md](README.md) - Project overview and quick start
- [PROJECT.md](PROJECT.md) - Case study and portfolio piece
- [SETUP-GUIDE.md](SETUP-GUIDE.md) - This setup guide

### Online Resources
- [Webflow Documentation](https://webflow.com/learn)
- [Lenis Documentation](https://github.com/studio-freight/lenis)
- [Howler.js Documentation](https://github.com/goldfire/howler.js)
- [Netlify Documentation](https://docs.netlify.com/)

### Community Support
- [GitHub Issues](https://github.com/devtitus/Wunderkint-Website/issues)
- [Stack Overflow](https://stackoverflow.com)
- [Webflow Forum](https://forum.webflow.com/)

---

*Last updated: January 2026*