# stepanovic.xyz

Personal blog built with Hugo and hosted on GitHub Pages.

## Development

1. Install Hugo: `brew install hugo` (on macOS)
2. Run locally: `hugo server -D`
3. Build: `hugo`

## Features

- Lightweight and fast
- Responsive design
- Support for images
- Interactive hover tooltips
- Custom font styling
- Automated GitHub Pages deployment

## Adding Content

1. Create new posts: `hugo new posts/my-new-post.md`
2. Add images to `static/images/`
3. Customize styling in `themes/minimal-blog/layouts/_default/baseof.html`

## Deployment

The site automatically deploys to GitHub Pages when you push to the main branch.

## Custom Domain Setup

To use your custom domain:

1. Go to your GitHub repository settings
2. Navigate to Pages section
3. Set your custom domain to `stepanovic.xyz`
4. Update your DNS records to point to GitHub Pages:
   - Add CNAME record: `www` → `yourusername.github.io`
   - Add A records for apex domain:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`

## Local Development

```bash
# Install Hugo (macOS)
brew install hugo

# Clone and run
git clone <repo>
cd <repo>
hugo server -D

# Create new post
hugo new posts/my-new-post.md
```

## Customization

### Fonts
Edit the `font-family` in `themes/minimal-blog/layouts/_default/baseof.html` to change the typography.

### Colors
Modify the CSS variables in the `<style>` section of `baseof.html` to change the color scheme.

### Tooltips
Use this syntax for interactive tooltips:
```html
<span class="tooltip">hover text<span class="tooltiptext">tooltip content</span></span>
```

### Images
Add images to `static/images/` and reference them in markdown:
```markdown
![Alt text](/images/your-image.jpg)
```
