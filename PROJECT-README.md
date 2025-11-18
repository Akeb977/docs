# E-Commerce Email Template Design System

Professional, responsive email templates for e-commerce brands with full documentation and ready-to-use HTML code.

## 📁 Project Structure

```
/
├── email-templates/          # Documentation for each template
│   ├── overview.mdx         # Overview of all templates
│   ├── design-system.mdx    # Design guidelines & specs
│   ├── welcome-series/      # Welcome & onboarding emails
│   ├── transactional/       # Order confirmations, shipping, etc.
│   ├── promotional/         # Sales, launches, campaigns
│   └── retention/           # Abandoned cart, win-back, etc.
│
├── email-assets/            # All email assets
│   ├── reference-images/   # Your design reference images
│   ├── images/             # Production email images
│   ├── logos/              # Brand logos
│   └── copy/               # Email copy documents
│
├── email-html/              # HTML email templates
│   ├── templates/          # Complete email templates
│   └── snippets/           # Reusable components
│
└── docs.json               # Mintlify navigation config
```

## 🚀 Getting Started

### Step 1: Add Your Reference Images

1. Place your email design reference images in `/email-assets/reference-images/`
2. Name them descriptively: `welcome-email-reference.png`, `order-confirmation-reference.png`
3. These help document your design vision

### Step 2: Upload Your Assets

1. **Logos**: Add to `/email-assets/logos/`
   - Format: PNG with transparent background
   - Size: 300px x 100px (or proportional)

2. **Images**: Add to `/email-assets/images/`
   - Hero images: 1200px x 600px
   - Product images: 600px x 600px
   - Optimize to <150KB per image

3. **Copy**: Save to `/email-assets/copy/`
   - Format: .txt or .md files
   - Include subject lines, body copy, CTAs

### Step 3: Customize the HTML Templates

Each template documentation page includes:
- Full HTML code with inline CSS
- Responsive design (mobile + desktop)
- Comments showing where to add your content
- Placeholders for images, links, and copy

**Find templates in the documentation:**
- Navigate to the "Email Templates" tab
- Choose your template category
- Scroll to the HTML section
- Copy and customize

### Step 4: Replace Placeholders

In the HTML code, replace these placeholders:

```html
YOUR_LOGO_URL          → Your actual logo URL
YOUR_HERO_IMAGE_URL    → Your hero/banner image URL
YOUR_CTA_LINK_HERE     → Your call-to-action link
{{ORDER_NUMBER}}       → Dynamic variables from your ESP
{{CUSTOMER_NAME}}      → Dynamic variables from your ESP
```

### Step 5: Test Your Emails

Before sending:
- [ ] Test on Gmail (desktop + mobile)
- [ ] Test on Outlook (2016, 365)
- [ ] Test on Apple Mail (iOS + macOS)
- [ ] Test on Yahoo Mail
- [ ] Verify all links work
- [ ] Check images load properly
- [ ] Test with images blocked
- [ ] Validate HTML

### Step 6: Deploy

**Option A: Copy HTML to ESP**
- Copy the HTML code
- Paste into your email service provider (Mailchimp, Klaviyo, etc.)
- Replace merge tags with your ESP's syntax
- Send test emails

**Option B: Import to Figma**
- Copy the HTML
- Use an HTML to Figma plugin OR
- Manually recreate the design using HTML as reference
- Customize in Figma for client presentations
- Export and convert back to HTML if needed

## 📖 Documentation

This project uses Mintlify for documentation. To view locally:

```bash
# Install Mintlify CLI
npm i -g mintlify

# Run local dev server
mintlify dev
```

Then visit http://localhost:3000

## 🎨 Customization

### Update Brand Colors

Edit `/email-templates/design-system.mdx` and then find/replace in HTML:

```css
Primary:    #000000  → Your brand color
Secondary:  #666666  → Your accent color
Background: #F5F5F5  → Your background color
```

### Add New Templates

1. Create new .mdx file in appropriate category folder
2. Add to `docs.json` navigation
3. Include: preview, copy, HTML, assets needed, best practices

### Modify Design System

Update `/email-templates/design-system.mdx` with:
- Your typography rules
- Spacing system
- Color palette
- Component specs

## 🛠️ Template Types Included

### Welcome Series
- ✅ Welcome Email (with discount offer)
- Add more as needed

### Transactional
- ✅ Order Confirmation
- Add: Shipping notification, delivery confirmation

### Promotional
- ✅ Sale Announcement
- Add: New product launch, seasonal campaigns

### Retention
- ✅ Abandoned Cart (3-email sequence)
- Add: Win-back, re-engagement, loyalty

## 📝 Workflow for Each Email

1. **Design** → Upload reference image to document vision
2. **Copy** → Write and save finalized copy
3. **Assets** → Gather and optimize all images
4. **HTML** → Customize template HTML code
5. **Test** → Test across email clients
6. **Figma** → Create polished presentation version (optional)
7. **Deploy** → Upload to ESP and launch

## 🎯 Best Practices

### Email Design
- Keep under 600px width
- Use tables for layout (email standard)
- Inline all CSS
- Optimize images (<150KB each)
- Include alt text for all images
- Test with images disabled

### Copy
- Subject line: 40-50 characters
- Preheader: 85-100 characters
- Clear single CTA
- Mobile-friendly text size (min 16px)
- Scannable content

### Performance
- Total email size: <500KB
- Load time: <3 seconds
- Mobile-first design
- Accessibility (WCAG AA)

## 🔗 Resources

### Tools
- [TinyPNG](https://tinypng.com/) - Image compression
- [Litmus](https://litmus.com/) - Email testing
- [Can I Email](https://www.caniemail.com/) - CSS/HTML support
- [Really Good Emails](https://reallygoodemails.com/) - Inspiration

### Email Service Providers
- Mailchimp
- Klaviyo
- Sendgrid
- Customer.io
- Braze

### Testing
- Litmus
- Email on Acid
- Mail-tester (spam score)

## 📞 Support

For questions about:
- **Templates**: Check the template documentation page
- **Design System**: See `/email-templates/design-system.mdx`
- **Assets**: Read `/email-assets/README.md`

## 🎨 Figma Integration

### Method 1: Plugin (Easiest)
1. Install "HTML to Figma" plugin
2. Copy HTML code from template
3. Paste into plugin
4. Adjust as needed

### Method 2: Manual (Most Control)
1. Use HTML as reference
2. Recreate design in Figma
3. Use exact measurements from CSS
4. Export for presentations

### Method 3: Screenshots
1. Send test email to yourself
2. Screenshot in email client
3. Import to Figma as reference
4. Design presentation version

## 📊 Tracking Performance

Key metrics to monitor:
- **Open Rate**: 15-25% is good for e-commerce
- **Click Rate**: 2-5% is good
- **Conversion Rate**: 1-3% is good
- **Revenue Per Email**: Track ROI

## 🚀 Next Steps

1. Start with the Welcome Email template
2. Add your brand assets
3. Customize the HTML
4. Test thoroughly
5. Deploy and measure results
6. Iterate based on performance

## 📄 License

Customize these templates freely for your e-commerce brand or client projects.

---

**Ready to create amazing emails?** Start with the [Email Templates Overview](/email-templates/overview)
