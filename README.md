# Incomplete Developer - Moonwalk Theme

A minimalist blog powered by Jekyll's Moonwalk theme with a custom modern light blue menu.

🌐 **Live Site:** [https://mpholoane-bapela.github.io](https://mpholoane-bapela.github.io)

## Features

- ✨ Clean minimalist design
- 🎨 Custom modern light blue gradient menu
- 🌓 Light/dark mode toggle
- 📱 Fully responsive
- ⚡ Super fast loading
- 🎯 SEO optimized

## Local Development (Optional)

If you want to preview changes locally:

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000`

## Adding New Posts

Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`

Example: `2026-02-15-my-new-post.md`

```markdown
---
layout: post
author: Mpholoane Bapela
---

Your content here...
```

## Customization

### Change Menu Colors

Edit `assets/css/main.scss` and modify the gradient colors:

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

Try these alternatives:
- Ocean Blue: `linear-gradient(135deg, #1e3c72 0%, #2a5298 100%)`
- Mint: `linear-gradient(135deg, #11998e 0%, #38ef7d 100%)`
- Sunset: `linear-gradient(135deg, #fa709a 0%, #fee140 100%)`

### Update Site Info

Edit `_config.yml`:
- Change `title`, `author`, `description`
- Add your social media links
- Customize appearance settings

### Menu Items

Edit `_data/home.yml` to add/remove menu items

## Theme

This blog uses the [Moonwalk](https://github.com/abhinavs/moonwalk) theme by Abhinav Saxena with custom styling.

## License

Content is © Mpholoane Bapela. Theme is MIT licensed.
