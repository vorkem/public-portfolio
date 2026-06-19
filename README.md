# Mike Crumpton - Interactive CV Portfolio

A modern, interactive HTML CV portfolio with dark/light mode, expandable experience sections, and responsive design. Perfect for hosting on GitHub Pages with a custom domain.

## Features

✨ **Interactive Elements**
- Dark/Light mode toggle with persistent preference (localStorage)
- Expandable experience sections with smooth animations
- Smooth scroll navigation
- Intersection observer for fade-in animations on scroll

🎨 **Modern Design**
- Clean, professional layout
- Responsive grid-based skills section
- Timeline visualization for work experience
- Smooth transitions and hover effects
- Beautiful gradient accents

📱 **Responsive**
- Mobile-first design
- Optimized for all screen sizes
- Touch-friendly interactive elements

🖨️ **Print-Ready**
- Expands all sections when printing
- Optimized print styles

## Getting Started Locally

1. Clone or download this repository
2. Open `index.html` in your browser
3. No build process needed!

## Hosting on GitHub Pages with Custom Domain

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Create a new public repository named `yourusername.github.io` (or any name)
3. Clone the repository to your computer:
   ```bash
   git clone https://github.com/yourusername/yourusername.github.io.git
   cd yourusername.github.io
   ```

### Step 2: Add Your CV Files

Copy the files from this project into your repository:
- `index.html`
- `styles.css`
- `script.js`

### Step 3: Push to GitHub

```bash
git add .
git commit -m "Add interactive CV portfolio"
git push origin main
```

### Step 4: Enable GitHub Pages (if not automatic)

1. Go to your repository settings
2. Scroll to "Pages" section
3. Under "Source", select `main` branch
4. Click Save

Your site will be live at `https://yourusername.github.io` (or your custom repository URL)

### Step 5: Set Up Custom Domain (Optional)

#### If you own a domain:

1. **Go to your domain registrar** (GoDaddy, Namecheap, Route53, etc.)
2. **Add DNS records:**
   - Create an `A` record pointing to GitHub's IP addresses:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   
   OR
   
   - Create a `CNAME` record pointing to `yourusername.github.io`

3. **Configure GitHub Pages:**
   - Go to repository Settings → Pages
   - Under "Custom domain", enter your domain (e.g., `mikecrumpton.com`)
   - Check "Enforce HTTPS"
   - Click Save

4. **Wait for DNS propagation** (can take 24-48 hours)

#### Example DNS Setup:
```
Type    Name       Value
A       @          185.199.108.153
A       @          185.199.109.153
A       @          185.199.110.153
A       @          185.199.111.153
CNAME   www        yourusername.github.io
```

### Step 6: Enable HTTPS

Once your custom domain is set up:
1. Go to Settings → Pages
2. Check "Enforce HTTPS"
3. GitHub will automatically provision an SSL certificate

## Customization

### Update Content

Edit `index.html` to:
- Change personal details
- Add/remove experience
- Modify skills
- Update interests

### Change Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --primary-color: #0066cc;      /* Main accent color */
    --primary-dark: #0052a3;       /* Darker shade */
    --text-dark: #1a202c;          /* Text color */
    --bg-light: #ffffff;           /* Background */
    /* ... more variables */
}
```

### Modify Layout

- Skills grid: Change `grid-template-columns` in `.skills-container`
- Timeline: Adjust `--before` element styles
- Font: Update `font-family` in `body` selector

## Browser Support

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- IE11: ⚠️ Basic support (no CSS Grid, animations limited)

## Performance

- **No dependencies** - Pure HTML/CSS/JavaScript
- **Lightweight** - ~30KB total (HTML + CSS + JS)
- **Fast loading** - No external fonts or frameworks
- **SEO friendly** - Semantic HTML structure

## Future Enhancements

Want to upgrade? Consider:
- [ ] Convert to React for more interactivity
- [ ] Add project showcase section
- [ ] Implement contact form
- [ ] Add blog section
- [ ] Create PDF export functionality
- [ ] Add animations library (AOS, Framer Motion)

## License

Feel free to use this template for your own CV portfolio. No attribution required.

## Tips

- **Update frequently:** Keep your CV current with new skills and experiences
- **SEO:** Add meta descriptions and og: tags for social sharing
- **Analytics:** Add Google Analytics or similar to track visitors
- **Backup PDF:** Keep the PDF version for traditional applications
- **Email:** Make sure the email link works properly
- **Testing:** Test on mobile devices before deploying

---

Built with ❤️ using HTML, CSS, and JavaScript
