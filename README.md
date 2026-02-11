# Incomplete Developer - Chirpy Theme

A customized Chirpy Jekyll theme for a C# & .NET development blog.

🌐 **Live Site:** [https://mpholoane-bapela.github.io](https://mpholoane-bapela.github.io)

## ✨ Custom Features

1. ✅ **Your photo as avatar**
2. ✅ **Custom social links:** YouTube, LinkedIn, Upwork, GitHub
3. ✅ **Bigger fonts** - All text increased
4. ✅ **Salmon pink headings** (#FF9999)

## 🚀 Installation (3 Steps)

### Step 1: Upload Files
1. Delete all old files from your repository
2. Upload ALL files from unzipped folder (including `.github` folder!)

### Step 2: Change GitHub Pages Settings ⚠️ IMPORTANT
1. Go to **Settings** → **Pages**
2. Under **Source**, change to: **"GitHub Actions"**
3. Save

### Step 3: Wait for Build
1. Go to **Actions** tab
2. Watch "Build and Deploy" run (3-5 minutes)
3. Green checkmark ✅ = Site is live!

## ⚙️ Update Before Publishing

Edit `_config.yml` and `_data/contact.yml` with your:
- LinkedIn URL
- YouTube URL  
- Upwork URL

## 📝 Adding Posts

Create: `_posts/2026-02-15-title.md`

```markdown
---
title: Your Title
date: 2026-02-15 10:00:00 +0200
categories: [C#]
tags: [dotnet]
---

Content here...
```

Commit → GitHub Actions rebuilds automatically!

## 🐛 Troubleshooting

**Build failing?**
- Check Actions tab for errors
- Verify `.github` folder uploaded
- Confirm Pages source = "GitHub Actions"

**Site not showing?**
- Wait 5 minutes after green checkmark
- Hard refresh (Ctrl + Shift + R)

---

**Happy blogging! 🚀**
