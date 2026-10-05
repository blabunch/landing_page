# NOTHING Landing Page

A responsive landing page for **NOTHING**, a London-based consumer tech brand. It presents the company's flagship products, its product categories, a short story about the brand, and a contact form.

🔗 **Live demo:** [blabunch.github.io/landing_page](https://blabunch.github.io/landing_page/)

## Project Description

NOTHING Landing Page is a single-page website that introduces visitors to the NOTHING brand and its minimalist tech products. The page is built mobile-first and scales from phones up to desktop screens.

It includes these sections:

- **Header:** the brand logo, a clickable phone number, a burger menu and the hero heading *"Bring joy back to the everyday"*.
- **Navigation menu:** a full-screen overlay with links to every section of the page and a "call to order" button. It is built with pure CSS (the `:target` pseudo-class), so it works without JavaScript.
- **Recommended:** product cards for Phone (1), Ear (2) and Ear (stick), each with an image, a description and a price.
- **Browse by category:** an image gallery that combines wide and square images for the *All products*, *Audio* and *Accessories* categories.
- **Banner:** a full-width image banner.
- **About us:** the brand's mission and values.
- **Contact us:** a feedback form (name, email, message) next to the company's phone, email and address. The address links to Google Maps.

The layout follows the **BEM** methodology. Each block has its own SCSS file, and shared values such as colors, breakpoints and spacing are kept in variables and mixins.

## Technical Requirements

To run this project locally, you need:

- **Node.js** (version 18.x or newer): the JavaScript runtime used by the build tools and linters.
- **npm** (version 9.x or newer): the Node.js package manager, used to install dependencies and run project scripts.
- **Git**: to clone the repository.

## Installation and Setup

1. **Clone the repository:**
    ```bash
    git clone https://github.com/blabunch/landing_page.git
    ```

2. **Go to the project directory:**
    ```bash
    cd landing_page
    ```

3. **Install dependencies:**
    ```bash
    npm install
    ```

4. **Start the local development server:**
    ```bash
    npm start
    ```

## Usage

After `npm start`, the development server opens the page in your browser and prints the local URL in the terminal. Changes to files in `src/` reload in the browser automatically.

Available scripts:

| Command | Description |
| --- | --- |
| `npm start` | Runs the development server with live reload |
| `npm run build` | Builds an optimized production version into the `dist/` folder |
| `npm run lint` | Checks HTML, SCSS and JavaScript with the linters |
| `npm test` | Runs the linters and the tests |
| `npm run deploy` | Builds the project and publishes it to GitHub Pages |

### Project Structure

```
src/
├── index.html              # Page markup
├── icon/                   # SVG/PNG icons (phone, burger menu, close)
├── images/                 # Logo, banner, product and category images
├── scripts/
│   └── main.js             # JavaScript entry point
└── styles/
    ├── main.scss           # Styles entry point: imports utils and blocks
    ├── utils/
    │   ├── variables.scss  # Colors, breakpoints, transition timing
    │   └── mixins.scss     # on-tablet, on-desktop, page-grid, hover, content-padding
    └── blocks/             # One file per BEM block (header, menu, product, store, ...)
```

## Features

- **Responsive design:** a mobile-first layout with breakpoints for tablet (≥ 576px) and desktop (≥ 1024px).
- **Grid-based layout:** a reusable `page-grid` mixin builds a CSS Grid with 2 columns on mobile and 6 columns on tablet and desktop.
- **Menu without JavaScript:** the burger menu opens and closes with the CSS `:target` pseudo-class. While it is open, page scrolling is locked with `:has()`.
- **Smooth interactions:** hover and focus effects with consistent transition timing.
- **Contact options:** clickable `tel:` and `mailto:` links, a map link for the address, and a contact form with built-in HTML validation.
- **Maintainable styles:** BEM naming, SCSS variables and mixins, and one file per component.
- **Code quality:** ESLint, Stylelint and LintHTML check the code, and Prettier formats it.

## Example

The live version of the project is available here: **[DEMO LINK](https://blabunch.github.io/landing_page/)**

## Technologies Used

- **HTML5:** semantic page structure (`header`, `nav`, `main`, `section`, `article`, `footer`) and form validation.
- **CSS3:** CSS Grid, Flexbox, transitions, and the `:target` and `:has()` selectors.
- **Sass (SCSS):** variables, mixins, nesting and partials, so the styles are easy to maintain.
- **BEM:** a naming methodology for predictable, reusable class names.
- **Parcel:** a zero-configuration bundler for the dev server and production builds (run through `@mate-academy/scripts`).
- **ESLint, Stylelint, LintHTML, Prettier:** linting and code formatting.
- **Google Fonts:** the *Space Grotesk* and *Space Mono* typefaces.
- **Git and GitHub:** version control and repository hosting.
- **GitHub Pages:** hosting for the live demo.

## Contribution Guidelines

If you would like to contribute to this project:

1. **Fork the repository:** create your own copy of the project on GitHub.
2. **Clone your fork:** download your copy to your computer.
3. **Create a branch:** make your feature or fix on a separate branch (`git checkout -b feature/your-feature`).
4. **Check your code:** run `npm test` to make sure the linters pass.
5. **Submit a pull request:** describe your changes and open a PR to the `master` branch.

## Author

**Bohdan Labunets**: [GitHub](https://github.com/blabunch)

## License

This project is licensed under the **GPL-3.0** License. See the [LICENSE](LICENSE) file for details.
