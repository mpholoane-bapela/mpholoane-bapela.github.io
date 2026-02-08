# Incomplete Developer - Chirpy Theme

A customized Chirpy Jekyll theme for a C# & .NET development blog.

🌐 **Live Site:** [https://mpholoane-bapela.github.io](https://mpholoane-bapela.github.io)

## ✨ Custom Features

All customizations you requested:

1. ✅ **Your photo as avatar** - Located in `/assets/img/avatar.png`
2. ✅ **Custom social links:**
   - YouTube (red icon) instead of Twitter
   - LinkedIn (blue icon) instead of Email  
   - Upwork (green icon) instead of RSS
   - GitHub (kept)
3. ✅ **Bigger fonts** - All text increased by ~2px throughout
4. ✅ **Salmon pink headings** - All H1, H2, H3 are #FF9999

## 🚀 Installation

### Method 1: GitHub Web Interface (Easiest)

1. **Delete old files** from your repository (or delete & recreate repo)
2. **Upload all files** from the unzipped folder
3. **Enable GitHub Pages:**
   - Settings → Pages
   - Source: Deploy from a branch
   - Branch: main
   - Save
4. **Wait 3-5 minutes** for the site to build

### Method 2: Git Command Line

```bash
git clone https://github.com/mpholoane-bapela/mpholoane-bapela.github.io.git
cd mpholoane-bapela.github.io
# Copy all files from this folder here
git add .
git commit -m "Install Chirpy theme with customizations"
git push
```

## ⚙️ Before Publishing - UPDATE THESE:

### 1. Social Media Links

Edit `_config.yml` and update:
```yaml
social:
  links:
    - https://github.com/mpholoane-bapela
    - https://linkedin.com/in/YOUR-USERNAME  # ← UPDATE
    - https://youtube.com/@YOUR-CHANNEL      # ← UPDATE
    - https://upwork.com/freelancers/~YOUR-ID # ← UPDATE
```

Also edit `_data/contact.yml` with the same URLs.

### 2. About Page

Edit `_tabs/about.md` and update your:
- Bio
- Tech stack
- Social links at the bottom

## 📝 Adding New Posts

Create files in `_posts/` with format: `YYYY-MM-DD-title.md`

Example: `_posts/2026-02-15-my-csharp-tutorial.md`

```markdown
---
title: My C# Tutorial
date: 2026-02-15 10:00:00 +0200
categories: [C#, Tutorials]
tags: [csharp, dotnet, beginners]
---

Your content here...

## Code Example

```csharp
public class Example 
{
    public void Hello() 
    {
        Console.WriteLine("Hello World!");
    }
}
```
\```

Markdown text continues...
```

## 🎨 Further Customization

### Change Heading Color

Edit `assets/css/jekyll-theme-chirpy.scss`:
```css
h1, h2, h3, h4, h5, h6 {
  color: #YOUR-COLOR !important;
}
```

### Change Font Sizes

Edit the same file and adjust:
```css
body {
  font-size: 18px !important; /* Change this number */
}
```

### Change Social Icon Colors

Edit `assets/css/jekyll-theme-chirpy.scss` and find the social icons section.

### Replace Avatar

Replace `/assets/img/avatar.png` with your new photo (keep it square, ~500x500px works best).

## 📂 File Structure

```
├── _config.yml          # Main configuration
├── _data/
│   └── contact.yml      # Social links
├── _posts/              # Your blog posts go here
├── _tabs/               # Main navigation pages
│   ├── about.md
│   ├── archives.md
│   ├── categories.md
│   └── tags.md
├── assets/
│   ├── css/
│   │   └── jekyll-theme-chirpy.scss  # Custom styles
│   └── img/
│       └── avatar.png   # Your photo
├── Gemfile
└── .gitignore
```

## 📚 Resources

- [Chirpy Documentation](https://chirpy.cotes.page/)
- [Chirpy GitHub](https://github.com/cotes2020/jekyll-theme-chirpy)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)

## 🐛 Troubleshooting

**Site not showing?**
- Wait 5 minutes for GitHub to build
- Check Settings → Pages is enabled
- Make sure branch is set to "main"

**Styles not applying?**
- Clear browser cache
- Check `/assets/css/jekyll-theme-chirpy.scss` exists
- Wait a few minutes after pushing changes

**Avatar not showing?**
- Make sure file is at `/assets/img/avatar.png`
- Check file size (keep under 1MB)
- Try refreshing with Ctrl+F5

## 📄 License

- Content: © Mpholoane Bapela
- Theme: MIT License (Chirpy)

---

**Happy blogging! 🚀**
