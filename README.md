# goit-markup-hw-06

Homework assignment #6 from the [GoIT](https://goit.global/) HTML/CSS markup course. Building on homework #5, this task makes the "Webstudio" landing page fully **responsive** (mobile, tablet, and desktop breakpoints) and adds JavaScript to make the mobile navigation menu and the "call back" modal actually open and close.

## 📋 About

The page is a fully responsive business landing for a fictional web studio. Compared to the previous homework, this version adds:

- **Responsive layout** with CSS media queries for mobile, tablet (`min-width: 768px`), and desktop (`min-width: 1158px`) breakpoints.
- **Retina-ready images**: separate `mobile/`, `tablet/`, and `main/` (desktop) image sets, each with standard and `-2x` (high-DPI) versions, served via `@media (min-resolution: 2x)` rules.
- A **mobile navigation menu**: a burger button (`data-menu-open`) opens a full-screen mobile menu overlay (`data-menu`), closed via a close button (`data-menu-close`).
- **Working JavaScript** for both the mobile menu (`js/menu.js`) and the "call back" modal (`js/modal.js`), toggling an `is-open` class on click.

The page itself still includes:

- A header with a logo, main navigation (Studio / Portfolio / Contacts), contact links, and (on mobile) a burger menu button.
- A hero section with a background image, heading, and an "Order Service" button that opens the modal.
- An "Our Features" section listing four company strengths, each with an icon.
- An "Our Team" section presenting four team members with photos, names, roles, and social links.
- An "Our Portfolio" section showcasing six sample projects with images, overlay descriptions, titles, and categories.
- A footer with the logo, a tagline, social media links, and a newsletter subscribe form.
- A modal dialog for leaving contact details, and a full-screen mobile navigation menu.

## 🛠️ Tech Stack

- HTML5 (semantic elements: `header`, `nav`, `main`, `section`, `address`, `footer`)
- CSS3 — responsive layout with media queries, retina image support
- Vanilla JavaScript — mobile menu and modal open/close logic
- SVG sprite (`images/icons.svg`) for scalable icons
- [modern-normalize](https://github.com/sindresorhus/modern-normalize) (via CDN) for CSS resets
- Google Fonts (Raleway, Roboto)

## 📁 Project Structure

```
goit-markup-hw-06-main/
├── css/
│   └── styles.css        # Page styles, including responsive media queries
├── js/
│   ├── menu.js             # Mobile navigation menu open/close logic
│   └── modal.js              # "Call back" modal open/close logic
├── images/
│   ├── icons.svg              # SVG icon sprite
│   ├── main/                    # Desktop images (1x and 2x)
│   ├── tablet/                    # Tablet images (1x and 2x)
│   └── mobile/                      # Mobile images (1x and 2x)
└── index.html                         # Page markup
```

## 🚀 Getting Started

No build step is required — just open `index.html` in a browser (an internet connection is needed to load the Google Fonts and the normalize.css CDN link). For best results with a local dev server (e.g. VS Code's Live Server), serve the folder rather than opening the file directly, so relative script/image paths resolve correctly.
