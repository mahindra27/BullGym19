# Bull Gym - Deployment Guide

## 🚀 Push to GitHub

Your project is ready to push! Follow these steps:

### Option 1: Create New Repository on GitHub (Recommended)

1. **Go to GitHub** and create a new repository:
   - Repository name: `bull-gym-website` (or any name you prefer)
   - Description: "Bull Gym Kuala Lumpur - Aggressive dark theme fitness website"
   - Keep it **Public** (for GitHub Pages hosting)
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)

2. **Copy the repository URL** from GitHub (should look like: `https://github.com/mahindra27/bull-gym-website.git`)

3. **Run these commands** in your terminal:

```bash
# Add your GitHub repository as remote origin
git remote add origin https://github.com/mahindra27/YOUR-REPO-NAME.git

# Rename branch to main (GitHub standard)
git branch -M main

# Push to GitHub
git push -u origin main
```

### Option 2: Push to Existing Repository

If you already have a repository:

```bash
git remote add origin YOUR-EXISTING-REPO-URL
git branch -M main
git push -u origin main
```

---

## 🌐 Deploy to GitHub Pages (Free Hosting)

After pushing to GitHub:

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in the left sidebar)
3. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes, then visit: `https://mahindra27.github.io/YOUR-REPO-NAME`

Your website will be live! 🎉

---

## 📦 Project Files Committed

✅ **index.html** - Main website (41KB)
✅ **README.md** - Complete documentation (18KB)
✅ **logo.jpeg** - Bull Gym branding (16KB)
✅ **.gitignore** - Git ignore rules

**Note:** The `images/`, `node_modules/`, `.vs/`, `src/`, and `videos/` folders are excluded via `.gitignore` as they are not needed for the website.

---

## 🔄 Future Updates

When you make changes to the website:

```bash
# Check what files changed
git status

# Add all changes
git add .

# Commit with a message
git commit -m "Updated pricing section"

# Push to GitHub
git push
```

GitHub Pages will automatically update your live site within 1-2 minutes!

---

## 💡 Alternative Hosting Options

If you prefer other platforms:

### Netlify (Recommended for simplicity)
1. Sign up at [netlify.com](https://netlify.com)
2. Drag and drop your project folder
3. Your site is live instantly!
4. Free SSL certificate included

### Vercel
1. Sign up at [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Deploy with one click
4. Free SSL certificate included

---

## 📞 Need Help?

Contact Mahindra Prasad:
- GitHub: [@mahindra27](https://github.com/mahindra27)
- LinkedIn: [Mahindra Prasad](https://www.linkedin.com/in/mahindra-prasad-4b32b02ba)

---

**Built with passion for Bull Gym Kuala Lumpur** 💪🔥
