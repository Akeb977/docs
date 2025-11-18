# Upload Your Brand Logos Here

Store all logo variations for use in email templates.

## Logo Specifications

### Primary Logo
- **Format**: PNG with transparent background (preferred)
- **Dimensions**: 300px x 100px (or maintain aspect ratio)
- **Max File Size**: 50KB
- **Color**: Full color version

### Logo Variations Needed

```
logo-primary.png       # Full color, transparent background
logo-white.png         # White version (for dark backgrounds)
logo-black.png         # Black version (for light backgrounds)
logo-icon.png          # Icon/symbol only (optional)
```

## File Naming

Use clear, consistent naming:

```
✅ Good:
brand-logo-color.png
brand-logo-white.png
brand-logo-monochrome.png

✅ Also good:
logo-light.png
logo-dark.png

❌ Bad:
logo1.png
final_logo_v2.png
untitled.png
```

## Technical Requirements

### Format
- **PNG**: Preferred (supports transparency)
- **SVG**: Not well supported in email - convert to PNG
- **JPG**: Only if you need solid background

### Size
- **Width**: 150-300px (will display at 150px typically)
- **Height**: 40-100px
- **Aspect Ratio**: Maintain brand proportions

### File Size
- Keep under 50KB
- Optimize using TinyPNG or similar tools

## Logo Placement in Emails

Logos typically appear:
1. **Header** - Top of email (most common)
2. **Footer** - Bottom of email (secondary)
3. **Invoice/Receipt** - Both header and footer

## Usage in HTML

In your email templates, reference like this:

```html
<!-- If hosting locally -->
<img src="/email-assets/logos/logo-primary.png"
     alt="Brand Name"
     width="150"
     style="display: block; height: auto;">

<!-- If hosting on CDN (production) -->
<img src="https://your-cdn.com/logo-primary.png"
     alt="Brand Name"
     width="150"
     style="display: block; height: auto;">
```

## Dark Mode Considerations

Some email clients support dark mode. Have both versions ready:

```html
<!-- Light mode logo (hidden in dark mode) -->
<img src="logo-dark.png" class="light-mode-logo" alt="Brand">

<!-- Dark mode logo (hidden in light mode) -->
<img src="logo-white.png" class="dark-mode-logo" alt="Brand">
```

## Optimization Checklist

Before using your logo in emails:

- [ ] Transparent background (if PNG)
- [ ] Correct dimensions (150-300px wide)
- [ ] Optimized file size (<50KB)
- [ ] Multiple versions prepared (color, white, black)
- [ ] Alt text = your brand name
- [ ] Tested on light AND dark backgrounds

## Common Issues

### Logo too small in email
- Use 2x size (300px) and display at 150px for retina screens

### Logo looks pixelated
- Use higher resolution PNG
- Ensure you're starting with vector (SVG) and exporting to PNG

### Logo takes too long to load
- Compress the file
- Use JPG if PNG is too large (but lose transparency)

## Tools & Resources

### Optimization
- [TinyPNG](https://tinypng.com/) - Compress PNGs
- [Squoosh](https://squoosh.app/) - Advanced compression

### Conversion
- [CloudConvert](https://cloudconvert.com/) - SVG to PNG
- Adobe Illustrator, Figma, or Sketch for exporting

### Testing
- Test logo on white background
- Test logo on colored backgrounds
- Test logo with images disabled

---

**Quick Tip**: Always export at 2x resolution for retina displays, then scale down in HTML using width attribute.
