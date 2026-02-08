# Incomplete Developer Blog

A personal blog about C# & .NET development, tech tutorials, and personal projects.

🌐 **Live Site:** [https://mpholoane-bapela.github.io](https://mpholoane-bapela.github.io)

## About

This blog is built with Jekyll and hosted on GitHub Pages. It focuses on:
- C# & .NET development
- Tech tutorials and learning resources
- Personal projects and experiments

## Getting Started

### 1. Clone this repository
```bash
git clone https://github.com/mpholoane-bapela/mpholoane-bapela.github.io.git
cd mpholoane-bapela.github.io
```

### 2. Enable GitHub Pages
1. Go to **Settings** → **Pages**
2. Under **Source**, select **main** branch
3. Click **Save**
4. Your site will be published at `https://mpholoane-bapela.github.io`

### 3. Customize Your Blog
- Edit `_config.yml` to update site settings
- Update `about.md` with your information
- Add your email and social media links

### 4. Add New Blog Posts
Create a new file in the `_posts` directory with this format:
```
_posts/YYYY-MM-DD-title-of-post.md
```

Example post structure:
```markdown
---
layout: post
title: "Your Post Title"
date: 2026-02-08 10:00:00 +0200
categories: [category1, category2]
tags: [tag1, tag2]
---

Your content here...
```

## Local Development (Optional)

To preview your site locally before pushing to GitHub:

1. Install Ruby and Bundler
2. Run:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
3. Visit `http://localhost:4000`

## Writing Posts

Posts are written in Markdown and stored in the `_posts` folder. The filename must follow the format: `YYYY-MM-DD-post-title.md`

### Front Matter
Each post needs front matter at the top:
```yaml
---
layout: post
title: "Your Title"
date: 2026-02-08 10:00:00 +0200
categories: [coding, dotnet]
tags: [csharp, tutorial]
---
```

### Markdown Syntax
- Headers: `#`, `##`, `###`
- Bold: `**text**`
- Italic: `*text*`
- Code: `` `code` ``
- Code blocks: ` ```language ```
- Links: `[text](url)`
- Images: `![alt](url)`

## Theme

This blog uses the [Minima](https://github.com/jekyll/minima) theme with the classic skin.

## License

Content is © Mpholoane Bapela. Feel free to reference or link to posts, but please don't republish without permission.

---

**Built with Jekyll and ❤️**
