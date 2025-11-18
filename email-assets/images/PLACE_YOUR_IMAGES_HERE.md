# Upload Your Production Email Images Here

This folder contains all images used in your actual email campaigns.

## Image Types & Specifications

### Hero/Banner Images
- **Size**: 1200px x 600px (displays at 600px width)
- **Format**: JPG (optimized)
- **Max File Size**: 150KB
- **Use**: Top banner, promotional headers

### Product Images
- **Size**: 600px x 600px (1:1 ratio)
- **Format**: JPG or PNG
- **Max File Size**: 100KB
- **Use**: Product showcases, cart items

### Category Images
- **Size**: 600px x 400px
- **Format**: JPG
- **Max File Size**: 100KB
- **Use**: Category tiles, collections

## File Naming Best Practices

Use descriptive, lowercase names with hyphens:

```
✅ Good:
hero-summer-sale-2024.jpg
product-blue-tshirt.jpg
category-womens-dresses.jpg

❌ Bad:
IMG_1234.jpg
photo.jpg
untitled.jpg
```

## Image Optimization

**Before uploading, optimize your images:**

1. **Resize** to correct dimensions (see specs above)
2. **Compress** using tools like:
   - [TinyPNG](https://tinypng.com/)
   - [Squoosh](https://squoosh.app/)
   - [ImageOptim](https://imageoptim.com/)
3. **Verify** file size is under limit
4. **Test** quality at display size

## Folder Organization (Optional)

You can create subfolders to organize:

```
/images
  /heroes
  /products
  /categories
  /banners
  /lifestyle
```

## Important Notes

### For Development
- Keep images in this folder during development
- Reference using relative or absolute paths

### For Production
- Upload to your CDN or email service provider
- Replace URLs in HTML templates
- Ensure HTTPS hosting (required for email)

### Alt Text
Always prepare descriptive alt text for each image:

```html
<!-- Good -->
<img src="product.jpg" alt="Blue cotton t-shirt, front view on white background">

<!-- Bad -->
<img src="product.jpg" alt="image">
```

## Checklist Before Using in Emails

- [ ] Correct dimensions for use case
- [ ] Optimized and compressed (<150KB)
- [ ] Descriptive filename
- [ ] Alt text written
- [ ] Hosted on reliable server (for production)
- [ ] HTTPS URL (for production)
- [ ] Tested in major email clients

## Quick Reference

| Image Type | Dimensions | Format | Max Size |
|------------|-----------|--------|----------|
| Hero | 1200x600px | JPG | 150KB |
| Product | 600x600px | JPG/PNG | 100KB |
| Category | 600x400px | JPG | 100KB |
| Icon | 64x64px | PNG | 10KB |

---

**Need help?** Check the [Design System](/email-templates/design-system) for complete guidelines.
