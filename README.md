# Birthday Wish — Interactive Celebration

A polished, responsive birthday surprise built with **HTML, CSS, and vanilla JavaScript**. Open the gift box, follow the animated letter journey, explore the cake and memory scenes, scratch the surprise vouchers, and enjoy the finale celebration.

## Live page

- **Website:** https://s1xer85.github.io/birthday-wish/
- **Repository:** https://github.com/s1xer85/birthday-wish

> The page is static and has no build step or server-side dependencies.

## Highlights

- Interactive gift-box opening sequence
- Resource-aware loading screen that waits for images, fonts, and the browser `load` event before starting the experience
- Responsive layout for desktop, tablet, and mobile screens
- Animated birthday letter and multi-stage celebration journey
- 3D-style cake and candle interaction
- Memory/photo card scenes using the included image assets
- Scratch-off surprise voucher cards
- Confetti, fireworks, petals, and smaller floating celebration balloons
- Heart balloons removed from the ambient balloon system for a cleaner visual style
- Regular balloon dimensions reduced by 50% in this variant
- Reduced-motion support for visitors who prefer fewer animations

## Project structure

```text
birthday-wish/
├── index.html              # Complete app markup, styling, and JavaScript
├── image/                  # Backgrounds, decorations, cake, gift, and photos
├── flower.jpg              # Memory scene image
├── image.jpg               # Memory scene image
├── .nojekyll               # Allows clean static hosting on GitHub Pages
└── README.md               # This documentation
```

## Run locally

No installation is required.

```bash
git clone https://github.com/s1xer85/birthday-wish.git
cd birthday-wish
python3 -m http.server 8000
```

Then open <http://localhost:8000> in a browser. A local server is recommended instead of opening the HTML file directly because it handles asset loading consistently.

## Customization

### Birthday message

Edit the `mockData` object in `index.html`:

```js
const mockData = {
  titleLetter: '🎂 Happy Birthday! 🎉✨',
  contentLetter: 'Your personalized birthday message...',
  signatureLetter: 'With love'
};
```

### Photos and artwork

Replace files in `image/` or update the corresponding image paths in `index.html`. Keep filenames unchanged for the simplest swap.

### Balloon styling

The balloon system is in the `FLOATING BALLOONS & CELEBRATION ATMOSPHERE` section. The regular balloon body is intentionally set to half the original width and height, and the heart-balloon branch has been removed in this variant.

### Loading behavior

The loader waits for:

1. All document images to finish loading or fail gracefully
2. Image decoding where supported
3. Web fonts to become ready where supported
4. The browser `load` event

Only after these checks does the loader disappear and the initial animations begin.

## Technology

- Semantic HTML5
- Modern CSS3 animations and responsive media queries
- Vanilla JavaScript
- [Anime.js](https://animejs.com/)
- [Bootstrap Grid](https://getbootstrap.com/)
- [Animate.css](https://animate.style/)
- [Font Awesome](https://fontawesome.com/)
- [Canvas Confetti](https://github.com/catdad/canvas-confetti)

External libraries are loaded from their public CDNs at runtime.

## Deployment

This repository is static and can be deployed to GitHub Pages, Netlify, Vercel, Cloudflare Pages, or any web server that serves `index.html` as the root document. GitHub Pages should use the `main` branch and `/` (root) directory.

## License

MIT License. The included photos and artwork should only be reused when you have permission to do so.
