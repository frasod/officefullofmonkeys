# Office Full of Monkeys 🐵

A landing page for showcasing projects and apps.

## Quick Start

1. Open `index.html` in your browser to preview
2. Edit `index.html` to add your actual project links
3. Customize `styles.css` to change colors/styling

## Deployment Options (All Free!)

### Option 1: GitHub Pages (Recommended)
1. Push this repo to GitHub
2. Go to repo Settings → Pages
3. Select "Deploy from branch" → main
4. Add your custom domain in the settings
5. Configure DNS at your registrar:
   - Add a CNAME record pointing to `yourusername.github.io`

### Option 2: Cloudflare Pages
1. Connect your GitHub repo to Cloudflare Pages
2. Deploy automatically
3. Add custom domain in Cloudflare dashboard

### Option 3: Netlify
1. Drag and drop this folder to netlify.com/drop
2. Add custom domain in settings

## Domain Transfer Tips

Your Wix domain ($60/2yr) is expensive! Consider transferring to:
- **Cloudflare** (~$10/yr) - at-cost pricing
- **Porkbun** (~$10/yr) - cheap & good
- **Namecheap** (~$12/yr)

To transfer:
1. Unlock domain at Wix
2. Get authorization code from Wix
3. Initiate transfer at new registrar
4. Confirm via email

## Customization

### Adding Projects
Edit `index.html` and update the project cards:
```html
<a href="YOUR_GITHUB_SPARKS_URL" class="project-card">
    <span class="project-icon">🎲</span>
    <h3>Your App Name</h3>
    <p>Description of your app</p>
</a>
```

### Changing Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary: #ff6b35;    /* Main accent color */
    --secondary: #f7c59f;  /* Background gradient */
    --dark: #2e2e2e;       /* Text color */
    --light: #fffaf5;      /* Light background */
}
```

## Files
- `index.html` - Main page structure
- `styles.css` - All styling
- `README.md` - This file

---
Made with 🍌 by monkeys
