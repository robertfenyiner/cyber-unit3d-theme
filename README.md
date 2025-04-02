# cyber-unit3D Theme 

![License](https://img.shields.io/badge/License-MIT-blue) 
![Version](https://img.shields.io/badge/Version-1.0.1-purple) 
![Compatibility](https://img.shields.io/badge/Platform-UNIT3D-darkcyan)

<p align="center">
  <img src="https://ptpimg.me/o11lqc.png" alt="Theme Preview" style="border-radius: 8px; border: 2px solid #775499;">
</p>

A sleek, cyberpunk-inspired CSS theme designed for UNIT3D.

---

<div style="border: 2px solid #775499; background-color: #1f1721; padding: 10px; border-radius: 5px; margin: 15px 0;">
  <strong>🔮 NOTE:</strong> For optimal appearance, set your profile settings to the <strong>"Dark Teal"</strong> theme.
</div>

---

### How to Install the Theme

1. **Navigate to**:  
   *User Icon (top-right corner) → **My Settings** → External CSS Stylesheet (Stacks on top of above theme)*

2. **Paste Theme URL**:  
   `http://rkeaves.online/css-theme/cyber.css`

3. **Set Base Theme**:  
   *Ensure your profile uses the **"Dark Teal"** theme for proper contrast ( General Settings → Style → Theme)*

4. **Activate Changes**:  
   Click **Save**  
   _Refresh page to apply_

<p align="center">
  <img src="https://ptpimg.me/401410.png" alt="Theme Preview" style="border-radius: 8px; border: 2px solid #775499;">
</p>


---

## Features
- **Cyberpunk Aesthetic**: Neon magenta/cyan accents, gradient overlays, and glowing borders
- **CSS Variables**: Easily customizable color scheme and layout settings
- **Responsive Design**: Media queries for chat components and mobile adaptability
- **Dynamic Effects**: 
  - Hover-based drop shadows 
  - Subtle pulse animations
  - Smooth transitions
- **Pre-Styled Components**:
  - Navigation bars
  - Torrent cards
  - Data tables
  - Chat boxes
  - Interactive panels
  - Cyberpunk-themed icons


---

## Configuration
Customize the theme by modifying these variables in `:root`:
```css
:root {
    --primary-accent: #775499;       /* Main purple */
    --secondary-accent: #6c5186;     /* Secondary purple */
    --cyber-magenta: #ff00ff;        /* Neon magenta */
    --cyber-cyan: #00ffff;           /* Neon cyan */
    --dark-base: #0c090f;            /* Background */
    --content-max-width: 1200px;     /* Page width */
    --quick-search-input-offset: 6px;/* Search bar positioning */
}
```

## Customization Guide

### 1. Color Scheme
Modify these core variables to change the theme's color profile:
- `--primary-accent`: Primary purple for borders/accents
- `--cyber-magenta`/`--cyber-cyan`: Neon highlights
- `--dark-base`: Base background color

### 2. Layout Adjustments
- `--content-max-width`: Max width of main content (default: 1200px)
- `--content-padding`: Horizontal padding of content container

### 3. Component Positioning
- `--quick-search-input-offset`: Vertical adjustment for search bar

---

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -m 'Add awesome feature'`)
4. Push to branch (`git push origin feature/improvement`)
5. Open a Pull Request

**Report issues here**:  
[https://github.com/RKeaves/rkeaves.github.io/issues](https://github.com/RKeaves/rkeaves.github.io/issues)

---

## Notes
- Tested on UNIT3D v9.0.1+
- [MIT License © 2024 RKeaves](https://opensource.org/licenses/MIT)
