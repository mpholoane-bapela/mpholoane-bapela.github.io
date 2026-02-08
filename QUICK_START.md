# Quick Start Guide - Incomplete Developer Blog

## 🚀 Deploy Your Blog in 5 Minutes

### Step 1: Upload Files to GitHub

You have all the files you need! Now upload them to your repository:

**Option A: Using Git Command Line**
```bash
# Navigate to your local folder
cd path/to/your/blog/folder

# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial blog setup with Jekyll"

# Add your GitHub repository as remote
git remote add origin https://github.com/mpholoane-bapela/mpholoane-bapela.github.io.git

# Push to GitHub
git push -u origin main
```

**Option B: Using GitHub Web Interface**
1. Go to https://github.com/mpholoane-bapela/mpholoane-bapela.github.io
2. Click **Add file** → **Upload files**
3. Drag and drop all these files
4. Click **Commit changes**

### Step 2: Enable GitHub Pages

1. Go to your repository settings: https://github.com/mpholoane-bapela/mpholoane-bapela.github.io/settings/pages
2. Under **Source**, select **main** branch
3. Click **Save**
4. Wait 2-3 minutes for GitHub to build your site

### Step 3: Visit Your Blog! 🎉

Your blog will be live at: **https://mpholoane-bapela.github.io**

---

## ✏️ Before You Publish - Customize These

### 1. Update `_config.yml`
- Change `email: your-email@example.com` to your real email (or remove the line)
- Add your social media links (Twitter, LinkedIn, etc.)

### 2. Update `about.md`
- Replace `your-email@example.com` with your actual email
- Add more about yourself

### 3. Optional: Edit Your First Post
- Located at `_posts/2026-02-08-welcome-to-incomplete-developer.md`
- Customize it to sound like you!

---

## 📝 How to Add New Blog Posts

1. Create a new file in the `_posts` folder
2. Name it: `YYYY-MM-DD-your-post-title.md` (e.g., `2026-02-15-my-first-csharp-tip.md`)
3. Add this at the top:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: 2026-02-15 10:00:00 +0200
   categories: [dotnet, tutorial]
   tags: [csharp, beginners]
   ---
   ```
4. Write your content in Markdown below the `---`
5. Save and push to GitHub
6. Your post will appear automatically!

---

## 🎨 Customize Further (Optional)

### Change Theme Colors
Edit `_config.yml` and change:
```yaml
minima:
  skin: classic  # Options: classic, dark, auto, solarized, solarized-dark
```

### Add More Pages
Create new `.md` files like `projects.md` or `contact.md` with:
```yaml
---
layout: page
title: Your Page Title
permalink: /page-url/
---
```

---

## ❓ Troubleshooting

**Site not showing up?**
- Wait 2-3 minutes after pushing
- Check Settings → Pages to ensure it's enabled
- Make sure you pushed to the `main` branch

**Changes not appearing?**
- GitHub Pages can take 1-2 minutes to rebuild
- Clear your browser cache

**Need help?**
- Check the README.md file
- Visit [Jekyll documentation](https://jekyllrb.com/docs/)
- GitHub Pages guide: https://docs.github.com/en/pages

---

**You're all set! Happy blogging! 🚀**
