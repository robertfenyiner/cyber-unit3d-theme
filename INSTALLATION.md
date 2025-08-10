# Cyber Unit3D Theme - Installation Guide for UNIT3D v9.1.5

## Quick Installation

### Method 1: Direct URL (Recommended)
1. **Login to your UNIT3D site**
2. **Navigate to**: User menu (top-right) → **My Settings**  
3. **Find**: "External CSS Stylesheet (Stacks on top of above theme)"
4. **Paste one of these URLs**:

   **Purple/Cyan Theme:**
   ```
   https://raw.githubusercontent.com/YourUsername/cyber-unit3d-theme/main/cyber-v9.1.5.css
   ```

   **Lime Green Theme:**
   ```
   https://raw.githubusercontent.com/YourUsername/cyber-unit3d-theme/main/cyber-lime-v9.1.5.css
   ```

5. **Set Base Theme**:
   - Purple theme: **"Dark Teal"** (Theme ID: 7)
   - Lime theme: **"Dark Green"** (Theme ID: 3)
6. **Click Save**
7. **Refresh the page**

### Method 2: Local Installation
1. **Download the CSS file** you want:
   - `cyber-v9.1.5.css` (purple/cyan)
   - `cyber-lime-v9.1.5.css` (lime green)
2. **Upload to your web server** (accessible via HTTP/HTTPS)
3. **Use the full URL** in the External CSS field
4. **Set the appropriate base theme**
5. **Save and refresh**

## Theme Compatibility

### ✅ Compatible with UNIT3D v9.1.5+
- Enhanced ratio bar
- Improved mobile navigation  
- Updated quick search
- Modern CSS variables
- Accessibility features

### ❌ Not compatible with older versions
- Use `cyber.css` for UNIT3D v9.0.4
- Some features may not work on v9.1.4 and below

## Theme Variants

### Purple/Cyan Theme (`cyber-v9.1.5.css`)
- **Primary Colors**: Purple (#775499), Cyan (#00ffff), Magenta (#ff00ff)
- **Base Theme**: Dark Teal
- **Style**: Classic cyberpunk with purple accents
- **Best for**: Traditional cyberpunk aesthetic

### Lime Green Theme (`cyber-lime-v9.1.5.css`)
- **Primary Colors**: Lime Green (#81C784), Neon Green (#39ff14), Matrix Green (#00ff41)
- **Base Theme**: Dark Green  
- **Style**: Matrix-inspired with green accents
- **Best for**: Matrix/hacker aesthetic

## Verification

### How to know it's working:
1. **Quick search bar** should have a purple/green border with glow effect
2. **Navigation dropdowns** should have cyberpunk styling
3. **Torrent cards** should have gradient backgrounds
4. **Ratio bar** (if visible) should have enhanced styling
5. **Hover effects** should show glowing borders

### If it's not working:
1. **Check the URL** is accessible in a new browser tab
2. **Verify base theme** is set correctly
3. **Clear browser cache** (Ctrl+F5 or Cmd+Shift+R)
4. **Check browser console** for any errors (F12 → Console)

## Mobile Testing

### Mobile-specific features:
- **Responsive ratio bar** that adapts to small screens
- **Enhanced mobile navigation** with touch-friendly elements
- **Optimized font sizes** for mobile viewing
- **Improved button spacing** for touch devices

### Test on mobile:
1. Open your UNIT3D site on mobile
2. Check the navigation menu
3. Test the search functionality
4. Verify chat and torrent pages

## Advanced Configuration

### Custom Color Scheme
You can customize colors by adding this CSS after the theme:

```css
:root {
  /* Change primary accent color */
  --primary-accent: #9966cc;
  
  /* Adjust glow intensity */
  --cyber-glow-intensity: 1.2;
  
  /* Modify border radius */
  --cyber-border-radius: 12px;
  
  /* Change animation speed */
  --cyber-transition-speed: 0.5s;
}
```

### Performance Optimization
For better performance:

1. **Host locally**: Download and host the CSS on your server
2. **Enable compression**: Use gzip compression on your web server
3. **Set cache headers**: Configure long cache times for CSS files
4. **Minify if needed**: Remove comments and whitespace for smaller files

### Accessibility Options
The theme includes accessibility features:

```css
/* Reduce motion for users who prefer it */
@media (prefers-reduced-motion: reduce) {
  /* Animations are automatically reduced */
}

/* High contrast mode support */
@media (prefers-contrast: high) {
  /* Colors are automatically enhanced */
}
```

## Troubleshooting

### Common Issues

**1. Theme not loading**
- Check if the URL is accessible
- Verify HTTPS if your site uses HTTPS
- Clear browser cache

**2. Partial styling**
- Wrong base theme selected
- Conflicting custom CSS
- Browser extension interference

**3. Mobile issues**
- Mobile browser cache
- Viewport meta tag missing
- Touch event conflicts

**4. Performance issues**
- Large CSS file size
- Slow server response
- Network connectivity

### Browser Support
- ✅ Chrome 90+
- ✅ Firefox 88+  
- ✅ Safari 14+
- ✅ Edge 90+
- ⚠️ Internet Explorer: Not supported

### Getting Help
1. **Check the logs**: Browser console (F12)
2. **Test in incognito**: Rule out extensions/cache
3. **Try different browser**: Isolate browser-specific issues
4. **Report issues**: [GitHub Issues](https://github.com/RKeaves/cyber-unit3d-theme/issues)

## Security Notes

### Safe Installation
- ✅ Using GitHub raw URLs is safe
- ✅ HTTPS URLs are preferred  
- ✅ CSS-only themes cannot execute JavaScript
- ⚠️ Only use trusted sources

### What the theme does:
- ✅ Changes visual styling only
- ✅ No data collection
- ✅ No external requests (except font loading)
- ✅ No JavaScript execution

### What it doesn't do:
- ❌ Access your data
- ❌ Modify site functionality
- ❌ Track your activity
- ❌ Make network requests

---

## Example Installation Script

For server administrators, here's a bash script to install locally:

```bash
#!/bin/bash
# Download and install Cyber Unit3D theme v2.0.0

THEME_DIR="/var/www/html/themes"
THEME_URL="https://raw.githubusercontent.com/YourUsername/cyber-unit3d-theme/main"

# Create theme directory
mkdir -p $THEME_DIR

# Download theme files
wget -O "$THEME_DIR/cyber-v9.1.5.css" "$THEME_URL/cyber-v9.1.5.css"
wget -O "$THEME_DIR/cyber-lime-v9.1.5.css" "$THEME_URL/cyber-lime-v9.1.5.css"

# Set permissions
chmod 644 $THEME_DIR/*.css
chown www-data:www-data $THEME_DIR/*.css

echo "Themes installed to $THEME_DIR"
echo "Use https://your-domain.com/themes/cyber-v9.1.5.css in UNIT3D settings"
```

---

**Installation Guide Version**: 2.0.0  
**Compatible with**: UNIT3D v9.1.5+  
**Last Updated**: August 2025
