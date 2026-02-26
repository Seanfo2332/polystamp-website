# PolyStamp & Print Services — Website

A modern, Mossery-inspired website with product pages. Built using principles from the [Claude Code UI Agents](https://github.com/mustafakendiguzel/claude-code-ui-agents) design system. Product structure referenced from [AE Print](https://www.aeprint.com.my/).

## What's Included

- **Mossery-style Layout** — Full-bleed hero, featured 2-col blocks, "Shop Our Products" grid
- **Products Page** — Categories: Rubber Stamps, Business Cards, Name Tags, Office Signs
- **Product Detail Pages** — Individual product specs, descriptions, WhatsApp quote CTA (no cart)
- **Clean Design** — Soft neutrals, minimal accent, Syne + DM Sans typography
- **3-Step Process** — "Custom Order in 3 Easy Steps" (Mossery-style)
- **Responsive** — Mobile-first with hamburger menu

## Adding Your Own Images

To add real product photos for the service cards:

1. Create an `images` folder
2. Add photos: `stamps.jpg`, `name-tags.jpg`, `business-cards.jpg`, `signs.jpg`
3. In `index.html`, update each `.service-card__image` div:

```html
<div class="service-card__image" style="background-image: url('images/stamps.jpg'); background-size: cover;"></div>
```

Or add to `styles.css`:
```css
.service-card:nth-child(1) .service-card__image {
  background: linear-gradient(rgba(0,0,0,0.1), rgba(0,0,0,0.1)), url('images/stamps.jpg') center/cover;
}
```

## Deployment

- **Google Sites**: Create a new site and embed the HTML, or use a custom HTML embed block
- **Netlify / Vercel**: Drag and drop the folder for free static hosting
- **GitHub Pages**: Push to a repo and enable Pages in settings

## Customization

Edit `styles.css` `:root` variables to change:
- `--color-accent` — Brand accent (default: gold #B8860B)
- `--color-bg` — Background color
- `--font-display` / `--font-body` — Typography

## Contact Links

All WhatsApp links point to: `https://wa.me/60167737910`
Update in `index.html` if your number changes.
