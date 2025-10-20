# 🚀 GitHub Setup Guide

This guide will help you push your Diwali AI Poster Generator to GitHub and set up GitHub Pages.

## 📋 Prerequisites

- GitHub account
- Git installed on your system
- Terminal/Command line access

## 🔧 Step-by-Step Instructions

### 1. Create GitHub Repository

1. Go to [GitHub](https://github.com)
2. Click the **+** icon in the top right corner
3. Select **New repository**
4. Repository settings:
   - **Repository name**: `diwali-ai-poster-generator`
   - **Description**: `Ultra-optimized AI script for creating personalized Diwali & Kali Pujo festival posters`
   - **Visibility**: ✅ Public (required for GitHub Pages)
   - **Initialize**: ❌ Do NOT initialize with README, .gitignore, or license (we already have these)
5. Click **Create repository**

### 2. Add GitHub Remote

```bash
# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR_USERNAME/diwali-ai-poster-generator.git

# Verify remote was added
git remote -v
```

**Replace `YOUR_USERNAME` with your actual GitHub username**

### 3. Push to GitHub

```bash
# Push your code to GitHub
git branch -M main
git push -u origin main
```

### 4. Enable GitHub Pages

#### Option A: Via GitHub Website (Recommended)

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**:
   - Select **Deploy from a branch**
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes for deployment
7. Your site will be live at: `https://YOUR_USERNAME.github.io/diwali-ai-poster-generator`

#### Option B: Via GitHub Actions

1. Create `.github/workflows/pages.yml`:
```yaml
name: Deploy GitHub Pages

on:
  push:
    branches: [ main ]

permissions:
  contents: read
  pages: write
  id-token: write

concurrency:
  group: "pages"
  cancel-in-progress: false

jobs:
  deploy:
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v3
      - name: Setup Pages
        uses: actions/configure-pages@v3
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v1
        with:
          path: '.'
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v1
```

2. Commit and push:
```bash
git add .github/workflows/pages.yml
git commit -m "Add GitHub Pages workflow"
git push
```

### 5. Verify Deployment

1. Go to your repository
2. Click **Actions** tab
3. Wait for "Deploy GitHub Pages" workflow to complete (green checkmark)
4. Visit your live site: `https://YOUR_USERNAME.github.io/diwali-ai-poster-generator`

## 📝 Update Repository Information

### Update Links in Files

After pushing, update these files with your actual GitHub username:

1. **README.md**: Replace `arjunghosh` with your username
2. **index.html**: Replace `arjunghosh` with your username
3. **LICENSE**: Update contact email if needed

```bash
# Quick find and replace (replace YOUR_USERNAME)
sed -i '' 's/arjunghosh/YOUR_USERNAME/g' README.md index.html
```

### Add Repository Topics

1. Go to your repository on GitHub
2. Click the gear icon next to **About**
3. Add topics:
   - `diwali`
   - `kali-pujo`
   - `ai-poster`
   - `festival`
   - `chatgpt`
   - `gemini`
   - `copilot`
   - `hindi`
   - `bengali`
   - `prompt-engineering`

## 🎨 Customize Your Site

### Update Contact Information

Edit `README.md` and `index.html` to update:
- Author name
- LinkedIn profile
- Email address
- Any other personal information

### Add Social Media Badges

Add to README.md:
```markdown
[![Twitter](https://img.shields.io/twitter/follow/YOUR_HANDLE?style=social)](https://twitter.com/YOUR_HANDLE)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Arjun%20Ghosh-blue)](https://linkedin.com/in/arjunghosh)
```

## 🔄 Future Updates

To update your repository:

```bash
# Make your changes
git add .
git commit -m "Description of changes"
git push
```

GitHub Pages will automatically redeploy within 1-2 minutes.

## 📊 Analytics (Optional)

### Add GitHub Stars Badge

```markdown
![GitHub stars](https://img.shields.io/github/stars/YOUR_USERNAME/diwali-ai-poster-generator?style=social)
```

### Add Visitor Counter

Add to README.md:
```markdown
![Visitor Count](https://visitor-badge.laobi.icu/badge?page_id=YOUR_USERNAME.diwali-ai-poster-generator)
```

## 🐛 Troubleshooting

### GitHub Pages Not Showing

1. Check **Settings** → **Pages** for deployment status
2. Verify branch is `main` and folder is `/ (root)`
3. Check **Actions** tab for any errors
4. Wait 5-10 minutes for initial deployment

### Push Errors

```bash
# If you get "remote origin already exists"
git remote set-url origin https://github.com/YOUR_USERNAME/diwali-ai-poster-generator.git

# If you get authentication errors
# Use GitHub CLI or SSH keys
gh auth login
```

### Files Not Showing

```bash
# Check what's tracked
git status

# Force add if needed
git add -f filename
git commit -m "Add missing file"
git push
```

## 📱 Share Your Project

### Social Media Template

```
🎉 Excited to share my new project!

🪔 Diwali AI Poster Generator
Create personalized Diwali & Kali Pujo festival posters with AI!

✨ Features:
• Works on ChatGPT, Gemini, Copilot
• Bilingual support (Hindi, Bengali)
• Ultra-optimized script
• Free & open source

🔗 Try it now: https://YOUR_USERNAME.github.io/diwali-ai-poster-generator

#AI #Diwali #OpenSource #Festival
```

## 📚 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Documentation](https://git-scm.com/doc)
- [Markdown Guide](https://www.markdownguide.org/)
- [Shields.io Badges](https://shields.io/)

## ✅ Checklist

- [ ] GitHub repository created
- [ ] Code pushed to GitHub
- [ ] GitHub Pages enabled
- [ ] Website is live
- [ ] README updated with correct links
- [ ] Repository topics added
- [ ] Social media post shared
- [ ] Analytics added (optional)

## 🎉 You're Done!

Your Diwali AI Poster Generator is now live on GitHub Pages!

**Live URL**: `https://YOUR_USERNAME.github.io/diwali-ai-poster-generator`
**Repository**: `https://github.com/YOUR_USERNAME/diwali-ai-poster-generator`

---

**Need Help?** Open an issue on GitHub or contact: arjun@example.com
