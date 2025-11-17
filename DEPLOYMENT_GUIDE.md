# 🚀 Quick Deployment Guide

## GitHub Pages Deployment (5 Minutes)

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the "+" icon → "New repository"
3. Name it: `sdwc-website` (or any name you prefer)
4. Choose "Public"
5. Don't initialize with README (we already have one)
6. Click "Create repository"

### Step 2: Push Your Code

Open terminal in the project folder and run:

```bash
# If you haven't already initialized git (already done):
# git init
# git branch -m main

# Add your GitHub repository as remote:
git remote add origin https://github.com/YOUR_USERNAME/sdwc-website.git

# Push your code:
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" (top right)
3. Click "Pages" (left sidebar)
4. Under "Source":
   - Select "Deploy from a branch"
   - Choose "main" branch
   - Choose "/ (root)" folder
5. Click "Save"

### Step 4: Access Your Website

Your site will be live at:
```
https://YOUR_USERNAME.github.io/sdwc-website/
```

⏱️ **First deployment takes 2-5 minutes**

---

## 📧 Mailchimp Email Signup Integration

### Quick Setup (5 Minutes)

1. **Create Mailchimp Account**: [mailchimp.com](https://mailchimp.com)

2. **Create Audience**:
   - Go to "Audience" → "Create Audience"
   - Fill in details

3. **Get Form Code**:
   - "Audience" → "Signup Forms" → "Embedded Forms"
   - Copy the form action URL (looks like):
     ```
     https://YOURDOMAIN.us1.list-manage.com/subscribe/post?u=XXXXX&id=YYYYY
     ```

4. **Update index.html**:
   - Find line ~205: `<form action="#"`
   - Replace `#` with your Mailchimp URL:
     ```html
     <form action="https://YOURDOMAIN.us1.list-manage.com/subscribe/post?u=XXXXX&id=YYYYY"
     ```

5. **Commit and Push**:
   ```bash
   git add index.html
   git commit -m "Add Mailchimp integration"
   git push
   ```

---

## 🔗 Important Links

- **Discord**: https://discord.gg/KWgEkXCCzY
- **Instagram**: https://instagram.com/sandiegowellnessclub
- **TikTok**: https://tiktok.com/@sandiegowellnessclub

---

## ✅ Pre-Deployment Checklist

- [x] All files are in the repository
- [x] Git repository initialized
- [x] All links tested locally
- [x] Responsive design verified
- [x] README.md included
- [x] Favicons included
- [ ] Mailchimp form integrated (optional - can be done after deployment)
- [ ] Custom domain configured (optional)

---

## 🛠️ Quick Fixes

### Links Not Working?
- Ensure all internal links use relative paths (no `/` at the start)
- Check that file names match exactly (case-sensitive)

### Images Not Showing?
- Verify images are in `images/` and `assets/` folders
- Check file names match exactly

### Styles Not Applied?
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check that Tailwind CDN is loading
- Verify `css/style.css` path is correct

---

## 📞 Need Help?

Join the Discord community: https://discord.gg/KWgEkXCCzY

---

**Ready to launch? Let's go! 🎉**

*Align. Connect. Thrive.*
