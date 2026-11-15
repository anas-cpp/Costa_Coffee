# ☕ Costa — Artisanal Coffee Roasters & Bakery Website

A responsive, single-file HTML5 website built for **Costa**, a specialty coffee roastery and neighborhood bakery. Designed with an editorial hospitality aesthetic using **Tailwind CSS**, **Google Fonts**, and **Vanilla JavaScript**—with zero build tools or external dependencies required.

---

## ✨ Key Features

- **Sticky Responsive Navigation:** Features brand identity, smooth anchor scrolling, a mobile hamburger drawer, a direct reservation trigger, and a live pickup cart item badge.
- **Full-Height Editorial Hero:** High-contrast hero showcase with ambient overlay, ethical sourcing badge, dual CTAs, and quick trust highlights.
- **About Us & Brand Story:** Dual-column photo collage, roasting heritage stats, and three core hospitality pillars (*Ethically Sourced*, *Artisanal Roast*, *Cozy Sanctuary*).
- **Interactive Filterable Menu:** Real-time category filtering (`All Items`, `Hot Coffee`, `Iced`, `Bakery`) with dynamic card rendering, pricing, tasting notes, and resilient image fallbacks.
- **Working Slide-Out Order Cart Drawer:**
  - Add items with animated toast notifications and badge pulse feedback.
  - Adjust item quantities (`+` / `−`) or remove items directly inside the drawer.
  - Automatic calculation of **Subtotal**, **Estimated Tax (8.5%)**, and **Total**.
  - Simulated pickup checkout flow with generated order confirmation numbers.
- **Customer Reviews Section:** Curated guest testimonials and verified rating highlights.
- **Location, Hours & Stylized Map Card:** Opening hours schedule, one-click address copy to clipboard, and an interactive neighborhood vector map with parking and transit toggles.
- **Table Reservation Modal:** Accessible booking modal with date/time selection, party size, input validation, and instant booking confirmation summary.
- **Cohesive Footer:** Quick navigation links, social icons, and a validated roastery newsletter signup form.

---

## 🎨 Design System & Color Palette

The interface uses a warm, tactile cafe color palette configured directly in the Tailwind CDN script:

| Token | Hex | Role |
| :--- | :--- | :--- |
| **Espresso** | `#2C1E16` | Primary text, dark surfaces, and primary action states |
| **Espresso Dark** | `#1E140E` | Hero gradient depth and footer background |
| **Cream** | `#FAF6F0` | Primary page canvas and modal surfaces |
| **Cream Dark** | `#F0E8DC` | Secondary section backgrounds and subtle button fills |
| **Caramel** | `#C87D55` | Brand accents, primary CTAs, badges, and price highlights |

### Typography
- **Headings:** [`Playfair Display`](https://fonts.google.com/specimen/Playfair+Display) — Editorial serif for titles, quotes, and pricing.
- **Body & UI:** [`Inter`](https://fonts.google.com/specimen/Inter) — Clean geometric sans-serif for navigation, descriptions, and controls.

---

## 🛠️ Tech Stack

- **Markup:** Semantic HTML5
- **Styling:** Tailwind CSS (v3 Play CDN with custom theme tokens)
- **Interactivity:** Vanilla ES6+ JavaScript (no frameworks or bundlers)
- **Imagery:** Curated Unsplash photography with automatic `placehold.co` fallback handling

---

## 🚀 Getting Started

Because the entire application is self-contained inside `index.html`, no installation or build step is needed:

1. **Clone or download** the project files into a local folder:
   ```text
   costa-cafe/
   ├── index.html
   └── README.md
   ```
2. **Open `index.html`** directly in any modern web browser (Chrome, Safari, Firefox, Edge), or serve it with a local static server such as VS Code Live Server or Python:
   ```bash
   python3 -m http.server 8080
   ```
3. Visit `http://localhost:8080` in your browser.

---

## 🧩 Customization Guide

- **Update Menu Items:** Edit the `MENU_ITEMS` array inside the `<script>` tag in `index.html` to add, remove, or modify drinks, pastries, prices, categories, or images.
- **Adjust Tax Rate:** Update the `0.085` multiplier inside the `renderCart()` function to match your local tax rate.
- **Edit Cafe Hours & Address:** Update the `#visit` section and the `copyCafeAddress()` helper function with your physical storefront details.

---

## 📄 License

This project is open-source and available for personal and commercial customization.
