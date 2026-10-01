# NOTHING — Landing Page

A responsive landing page for the **NOTHING** tech brand, built with semantic HTML, SCSS and the BEM methodology. Pure HTML + CSS, no frameworks — the mobile menu works without JavaScript.

🔗 **[Live demo](https://blabunch.github.io/landing_page/)**

## Features

- **Responsive layout** for mobile, tablet (≥ 576px) and desktop (≥ 1024px)
- **Mobile menu without JS**, using the CSS `:target` pseudo-class
- **CSS Grid** page layout (2 columns on mobile, 6 on tablet and up) built with a reusable SCSS mixin
- **BEM** class naming, with one SCSS file per block
- Smooth hover and focus effects
- Clickable phone links (`tel:`) and a contact form

## Page sections

| Section | Description |
| --- | --- |
| Header | Logo, phone number, burger menu and the hero heading |
| Menu | Full-screen navigation overlay |
| Recommended | Product cards: Phone (1), Ear (2), Ear (stick) |
| Stores | Product categories with a gallery of images |
| Banner | Full-width promo banner |
| About / Login | Information about the company |
| Contact us | Feedback form |
| Footer | Page footer |

## Tech stack

- HTML5
- SCSS (variables, mixins, partials)
- CSS Grid and Flexbox
- [Parcel](https://parceljs.org/) via `@mate-academy/scripts`
- Linters: ESLint, Stylelint, LintHTML, Prettier

## Project structure

```
src/
├── index.html
├── icon/              # SVG/PNG icons
├── images/            # Logo, banner, product and category images
├── scripts/
│   └── main.js
└── styles/
    ├── main.scss      # Entry point
    ├── utils/
    │   ├── variables.scss   # Colors, breakpoints
    │   └── mixins.scss      # on-tablet, on-desktop, page-grid, hover…
    └── blocks/        # One file per BEM block (header, menu, product, store…)
```

## Getting started

Requirements: [Node.js](https://nodejs.org/) (LTS) and npm.

```bash
git clone https://github.com/blabunch/landing_page.git
cd landing_page
npm install
npm start
```

## Scripts

| Command | Description |
| --- | --- |
| `npm start` | Start the dev server with live reload |
| `npm run build` | Build the production version |
| `npm run lint` | Check code with the linters |
| `npm test` | Run linters and tests |
| `npm run deploy` | Deploy to GitHub Pages |

## Author

**Bohdan Labunets** — [GitHub](https://github.com/blabunch)

## License

The project is distributed under the [GPL-3.0](LICENSE) license.
