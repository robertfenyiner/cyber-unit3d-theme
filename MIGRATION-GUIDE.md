# Migration Guide: Cyber Unit3D Theme v1.0.1 → v2.0.0

## Overview
This guide helps users migrate from the legacy cyber theme (v1.0.1) compatible with UNIT3D v9.0.4 to the new version (v2.0.0) compatible with UNIT3D v9.1.5+.

## Why Update?

### Issues Fixed in v2.0.0
- ✅ **Quick Search Input**: Fixed styling for the updated `.quick-search__input` class
- ✅ **Ratio Bar**: Added support for the new responsive ratio bar component
- ✅ **Icon Bar**: Enhanced mobile navigation with improved icon bar styling  
- ✅ **Data Tables**: Updated for new CSS variable system in v9.1.5
- ✅ **Dropdown Menus**: Fixed navigation dropdown positioning and styling
- ✅ **Mobile Responsiveness**: Better mobile layout support with new grid system
- ✅ **Accessibility**: Added support for reduced motion and high contrast preferences

### What Was Broken in v1.0.1 with UNIT3D v9.1.5
- Quick search input had incorrect styling due to class changes
- Ratio bar wasn't displaying properly on mobile devices
- Some hover effects weren't working on navigation elements
- Form controls had outdated variable references
- Missing support for new CSS custom properties

## Migration Steps

### Step 1: Update Theme URL
Replace your current theme URL in **My Settings** → **External CSS Stylesheet**:

**Old URL (v1.0.1):**
```
https://rkeaves.github.io/css-theme/cyber.css
```

**New URL (v2.0.0):**
```
https://your-domain.com/cyber-v9.1.5.css
```

### Step 2: Choose Your Variant
Select the appropriate theme for your preference:

**Purple/Cyan Theme (Default):**
- File: `cyber-v9.1.5.css`
- Base Theme: **Dark Teal**

**Lime Green Theme:**
- File: `cyber-lime-v9.1.5.css`  
- Base Theme: **Dark Green**

### Step 3: Update Base Theme
The recommended base themes remain the same:
- **Purple theme**: Dark Teal (ID: 7)
- **Lime theme**: Dark Green (ID: 3)

### Step 4: Clear Browser Cache
After updating:
1. Clear your browser cache (Ctrl+F5 or Cmd+Shift+R)
2. Save your settings again
3. Refresh the page

## New Features in v2.0.0

### Enhanced Components
- **Responsive Design**: Better mobile and tablet support
- **Modern Animations**: Smoother transitions with reduced motion support
- **Improved Typography**: Better font rendering with JetBrains Mono
- **Enhanced Chat**: Updated chatbox styling with better avatars

### New CSS Variables
v2.0.0 introduces new customization options:

```css
:root {
  --cyber-glow-intensity: 0.8;        /* Glow effect strength */
  --cyber-border-radius: 8px;         /* Universal border radius */
  --cyber-transition-speed: 0.3s;     /* Animation speed */
}
```

### Accessibility Improvements
- Support for `prefers-reduced-motion`
- Support for `prefers-contrast: high`
- Better keyboard navigation
- Improved color contrast ratios

## Customization Changes

### Updated Color Variables
Some color variables have been renamed for consistency:

**v1.0.1:**
```css
--quick-search-input-offset: 6px;
```

**v2.0.0:**
```css
--cyber-border-radius: 8px;          /* More flexible */
--cyber-transition-speed: 0.3s;      /* Configurable speed */
--cyber-glow-intensity: 0.8;         /* Adjustable glow */
```

### New Component Selectors
v2.0.0 adds styling for new UNIT3D v9.1.5 components:

```css
/* New in v2.0.0 */
.top-nav__ratio-bar { /* Responsive ratio bar */ }
.top-nav__icon-bar { /* Enhanced icon bar */ }
.quick-search__results { /* Search results dropdown */ }
```

## Troubleshooting

### Theme Not Loading
1. Check the URL is correct and accessible
2. Verify your base theme setting
3. Clear browser cache
4. Check browser console for errors

### Missing Styles
1. Ensure you're using UNIT3D v9.1.5+
2. Verify the theme URL points to the v2.0.0 files
3. Check if you have any conflicting custom CSS

### Mobile Issues
1. Clear mobile browser cache
2. Try disabling other browser extensions
3. Test in private/incognito mode

### Performance Issues
If you experience slow loading:
1. Host the CSS file locally for better performance
2. Enable browser caching
3. Use the reduced motion version if needed

## Backward Compatibility

### Staying on v1.0.1
If you need to stay on UNIT3D v9.0.4:
- Keep using `cyber.css` (original version)
- Do not update to v2.0.0 files
- The old theme will continue to work on v9.0.4

### Mixed Environments
If you have multiple UNIT3D instances:
- Use v1.0.1 files for v9.0.4 instances
- Use v2.0.0 files for v9.1.5+ instances
- Consider updating all instances to v9.1.5+ for consistency

## Support

### Getting Help
1. **GitHub Issues**: [Report bugs or request features](https://github.com/RKeaves/cyber-unit3d-theme/issues)
2. **Documentation**: Check the updated README.md
3. **Community**: Ask in UNIT3D community forums

### Contributing
The theme is open source and contributions are welcome:
- Fork the repository
- Create feature branches
- Submit pull requests
- Report issues

## Changelog Summary

### v2.0.0 (Current)
- ✅ UNIT3D v9.1.5+ compatibility
- ✅ Enhanced responsive design
- ✅ New accessibility features
- ✅ Improved performance
- ✅ Modern CSS architecture

### v1.0.1 (Legacy)
- ✅ UNIT3D v9.0.4 compatibility
- ✅ Basic cyberpunk styling
- ✅ Original color schemes

---

**Last Updated**: August 2025  
**Theme Version**: v2.0.0  
**UNIT3D Compatibility**: v9.1.5+
