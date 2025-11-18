# Email Assets Directory

This directory stores all assets used in your e-commerce email templates.

## Folder Structure

```
email-assets/
├── reference-images/    # Your design reference images
├── images/             # Production email images
├── logos/              # Brand logos
└── copy/               # Email copy documents
```

## How to Use

### 1. Reference Images
Upload your email design inspiration/reference images here:
- File naming: `[template-name]-reference.png`
- Example: `welcome-email-reference.png`
- These are for documentation and design reference only

### 2. Production Images
Upload optimized images for use in actual emails:
- **Hero images**: 1200px x 600px (will scale to 600px)
- **Product images**: 600px x 600px (1:1 ratio)
- **Category images**: 600px x 400px
- **Format**: JPG for photos, PNG for graphics with transparency
- **Optimization**: Compress to <150KB per image
- **Tools**: Use TinyPNG, ImageOptim, or Squoosh

### 3. Logos
Upload brand logos:
- **Format**: PNG with transparent background preferred
- **Size**: 300px x 100px (or proportional)
- **Versions**: Upload both light and dark versions if needed
- **File naming**: `logo-light.png`, `logo-dark.png`

### 4. Copy Documents
Save finalized email copy:
- **Format**: Plain text (.txt) or Markdown (.md)
- **File naming**: `[template-name]-copy.txt`
- **Include**: Subject lines, preheader, body copy, CTAs
- **Version control**: Update date in filename for revisions

## Image Hosting

### For Development/Testing
- Keep images in this folder
- Reference using relative paths in HTML

### For Production
Upload images to your preferred hosting:
- **Your website CDN**: Best for branding consistency
- **Email service provider**: (Mailchimp, Klaviyo have image hosting)
- **Cloud storage**: AWS S3, Cloudinary, imgix
- **CDN**: Use a CDN for faster global delivery

## Image Optimization Checklist

Before using any image in production emails:

- [ ] Compressed to smallest file size without quality loss
- [ ] Correct dimensions (see guide above)
- [ ] Descriptive alt text prepared
- [ ] Hosted on reliable, fast server
- [ ] HTTPS URL (required by most email clients)
- [ ] Tested display in major email clients
- [ ] Fallback color set for slow-loading images

## Best Practices

### File Naming
Use descriptive, lowercase names with hyphens:
- ✅ `hero-summer-sale-2024.jpg`
- ❌ `IMG_1234.jpg`

### Alt Text
Always write descriptive alt text for accessibility:
```html
<!-- Good -->
<img src="product.jpg" alt="Blue cotton t-shirt on white background">

<!-- Bad -->
<img src="product.jpg" alt="image">
```

### File Size Limits
- Single image: < 150KB
- Total email size: < 500KB (including all images)

### Image Formats
- **JPG**: Photos, hero images, lifestyle shots
- **PNG**: Logos, icons, graphics with transparency
- **GIF**: Avoid animated GIFs unless necessary (large file sizes)
- **SVG**: Not well supported in email - convert to PNG

## Quick Reference

| Asset Type | Dimensions | Format | Max Size |
|------------|-----------|--------|----------|
| Hero Image | 1200x600px | JPG | 150KB |
| Logo | 300x100px | PNG | 50KB |
| Product Image | 600x600px | JPG | 100KB |
| Category Image | 600x400px | JPG | 100KB |
| Icon | 64x64px | PNG | 10KB |
| Social Icon | 64x64px | PNG | 5KB |

## Tools & Resources

### Image Optimization
- [TinyPNG](https://tinypng.com/) - Free compression
- [Squoosh](https://squoosh.app/) - Advanced optimization
- [ImageOptim](https://imageoptim.com/) - Mac app

### Stock Photos
- [Unsplash](https://unsplash.com/)
- [Pexels](https://www.pexels.com/)
- Your own product photography

### Image Hosting
- Your website's media library
- Email platform's image hosting
- [Cloudinary](https://cloudinary.com/) - Free tier available
- [imgix](https://imgix.com/) - Image CDN

## Need Help?

Check the [Design System](/email-templates/design-system) for complete image guidelines and specifications.
