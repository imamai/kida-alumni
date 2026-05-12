# KIDA Alumni Website - Static HTML Version

This is a fully functional, responsive HTML website for the KIDA Alumni Association. It's ready to be hosted on GitHub Pages for free!

## 📁 Project Structure

```
html-website/
├── index.html           # Home page
├── about.html          # About page
├── events.html         # Events page
├── contact.html        # Contact page
├── register.html       # Registration & membership page
├── assets/
│   ├── styles.css      # All styling (compiled from Tailwind-like utilities)
│   └── script.js       # Interactive features (mobile menu)
└── README.md           # This file
```

## 🚀 Getting Started Locally

1. **Open in Browser**: Simply open `index.html` in your web browser to preview the site
2. **Live Server**: For best experience, use VS Code's Live Server extension:
   - Install: "Live Server" by Ritwick Dey
   - Right-click on `index.html` → "Open with Live Server"

## 📤 Hosting on GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Click **"New"** to create a new repository
3. Name it: `kida-alumni` or your preferred name
4. Make it **Public**
5. Click **"Create repository"**

### Step 2: Upload the Website

#### Option A: Using GitHub Web Interface
1. Click **"Add file"** → **"Upload files"**
2. Drag and drop the entire `html-website` folder contents
3. Commit with message: "Initial KIDA alumni website"

#### Option B: Using Git Commands
```bash
# Navigate to the html-website folder
cd html-website

# Initialize git
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial KIDA alumni website"

# Add remote repository (replace USERNAME and REPO)
git remote add origin https://github.com/USERNAME/REPO.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top right)
3. Scroll to **"Pages"** section (left sidebar)
4. Under **"Source"**, select **"main"** branch
5. Click **"Save"**
6. Wait 1-2 minutes for deployment
7. Your site will be live at: `https://USERNAME.github.io/REPO/`

## 🎨 Customization

### Update Content

- **index.html**: Edit the hero section and highlights
- **about.html**: Update mission statement and pillars
- **events.html**: Add/edit upcoming events
- **contact.html**: Update contact information
- **register.html**: Modify membership tiers and form fields

### Customize Colors

Edit the CSS variables in `assets/styles.css`:

```css
:root {
  --kida-navy: #2a4a7f;      /* Primary color */
  --kida-gold: #caa45f;      /* Accent color */
  --kida-ink: #0f172a;       /* Dark text */
}
```

### Update Contact Information

Replace these throughout the HTML files:
- Email: `alumni@kida.org`
- Phone: `+254 700 000 000`
- Address: `KIDA Campus Road, Nairobi, Kenya`

### Add a Contact Form Backend

The contact form uses FormSpree for email submissions:

1. Go to [formspree.io](https://formspree.io)
2. Sign up and create a new form
3. Get your form ID
4. In `contact.html`, replace `YOUR_FORM_ID` with your actual form ID:

```html
<form method="POST" action="https://formspree.io/f/YOUR_FORM_ID">
```

## 📱 Features

✅ Fully responsive (mobile, tablet, desktop)
✅ Fast loading (pure HTML/CSS)
✅ SEO optimized
✅ No dependencies needed
✅ Accessible (WCAG compliant)
✅ Mobile hamburger menu
✅ Font Awesome icons
✅ Professional design

## 🔧 Integration Options

### M-Pesa Payment Integration

The register page has placeholder M-Pesa functionality. To integrate real payments:

1. Sign up for [Daraja by Safaricom](https://developer.safaricom.co.ke)
2. Get your API credentials
3. Implement the M-Pesa STK push in a backend service
4. Update the registration form to call your backend

### Email Newsletter

To add newsletter functionality:
1. Use [Mailchimp](https://mailchimp.com) or similar service
2. Update the footer subscription form
3. Connect the form to your email service API

## 📊 Analytics

Add Google Analytics to track visitors:

1. Go to [google.com/analytics](https://google.com/analytics)
2. Create a property for your site
3. Get your measurement ID
4. Add this to the `<head>` of each HTML file:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 🐛 Troubleshooting

### Site not loading after pushing to GitHub
- Wait 2-3 minutes for GitHub Pages to deploy
- Check Settings → Pages to verify the source branch is set correctly
- Try clearing browser cache (Ctrl+Shift+Delete)

### Styles not appearing
- Ensure `assets/styles.css` and `assets/script.js` paths are correct
- Check browser console for 404 errors (F12)

### Mobile menu not working
- Check if JavaScript is enabled in browser
- Open browser console (F12) and check for errors

## 📝 License

This website template is free to use and modify for KIDA Alumni Association.

## 🎯 Next Steps

1. ✅ Upload to GitHub
2. ✅ Enable GitHub Pages
3. ✅ Share your live site URL
4. 📧 Integrate contact form backend
5. 💳 Integrate M-Pesa payments
6. 📊 Add analytics
7. 📰 Add news/blog section (optional)

---

**Questions?** Contact the development team or refer to GitHub Pages documentation at [pages.github.com](https://pages.github.com)
