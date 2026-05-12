# GitHub Setup Guide for KIDA Alumni Website

## Quick Start (5 minutes)

### 1. Create Repository on GitHub

```bash
# If you have Git installed, clone this command:
# Go to github.com, create new repo "kida-alumni"
```

### 2. Upload Files

**Using Web Browser:**
1. Go to your GitHub repository
2. Click "Upload files"
3. Drag the contents of `html-website` folder
4. Commit with message: "Add KIDA alumni website"

**Or Using Command Line:**
```bash
cd /path/to/html-website
git init
git add .
git commit -m "Add KIDA alumni website"
git remote add origin https://github.com/YOUR_USERNAME/kida-alumni.git
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages

1. Go to repository Settings
2. Scroll to "Pages"
3. Select "main" branch as source
4. Click Save
5. Wait 2-3 minutes
6. Your site is live at: `https://YOUR_USERNAME.github.io/kida-alumni/`

## File Structure for GitHub Pages

```
kida-alumni/
├── index.html
├── about.html
├── events.html
├── contact.html
├── register.html
├── assets/
│   ├── styles.css
│   └── script.js
└── README.md
```

## Updating Content

After setup, to update the website:

```bash
# Make changes to HTML files
nano index.html  # or edit in any text editor

# Push changes to GitHub
git add .
git commit -m "Update website content"
git push
```

## Custom Domain (Optional)

To use a custom domain like `alumni.kida.org`:

1. Buy a domain from a registrar (Namecheap, GoDaddy, etc.)
2. In repository Settings → Pages
3. Add your custom domain
4. Update DNS records at your registrar to point to GitHub

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Site not live after 5 min | Check Settings → Pages, verify main branch selected |
| 404 errors | Check file paths in HTML, ensure CSS/JS in assets folder |
| Styles not loading | Verify `assets/styles.css` exists, clear browser cache |
| Mobile menu broken | Ensure JavaScript is enabled, check browser console |

## File Size Reference

- Total site: ~50 KB (excellent for GitHub Pages)
- Each HTML page: 5-8 KB
- CSS file: 20 KB
- JavaScript: 1 KB

## Support

- GitHub Pages Docs: https://pages.github.com
- GitHub Desktop: https://desktop.github.com (GUI alternative to git)
- VS Code: Install "GitHub Pull Requests" extension for easier management

---

**Ready to go live?** Follow the 3 quick steps above and your KIDA alumni website will be accessible to everyone!
