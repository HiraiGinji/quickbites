# QuickBites

> A food delivery landing page and menu website with an animated splash screen and a rotating food carousel.

---

## Features

- **Animated splash screen**: the QuickBites logo slides in, then slides out and fades away on page load
- **Hero section**: bold headline with **Download** and **Order Now** call-to-action buttons
- **Food carousel**: circular food images with prev/next controls, where the active dish is enlarged and the others are blurred
- **Rotating text ring**: spinning "Fresh • Handmade • Healthy • Organic • Tasty • Delicious" text around the active dish
- **Menu page**: a separate `menu.html` for browsing food items
- **Responsive design**: layout and carousel sizes adapt across desktop, tablet, and mobile
- **Bootstrap navbar**: collapsible navigation with Home, Menu, Features, How It Works, and Contact links

## Tech Stack

- HTML5, CSS3, and vanilla JavaScript
- [Bootstrap 5.3.0](https://getbootstrap.com/) (via CDN)
- [Google Fonts: Poppins](https://fonts.google.com/specimen/Poppins)

## Project Structure

```
quickbites/
├── Images/        # Logos and food images
├── index.html     # Landing page (splash, hero, carousel)
├── menu.html      # Menu page
└── README.md
```

## Getting Started

No build step is required.

1. **Clone the repository**
   ```bash
   git clone https://github.com/HiraiGinji/quickbites.git
   cd quickbites
   ```

2. **Open the site**
   - Double-click `index.html`, **or**
   - Serve it locally:
     ```bash
     python -m http.server 8000
     ```
     Then visit `http://localhost:8000`.

> An internet connection is needed for the Bootstrap and Google Fonts CDNs.

## Customization

| What to change         | Where                                                      |
| ---------------------- | ---------------------------------------------------------- |
| Brand color (purple)   | `#51087E` and `#7e35b3` in the `<style>` block             |
| Accent color (yellow)  | `.order-button` styles (`#f1c40f`)                         |
| Hero headline & text   | `.hero-title` and `.hero-subtitle` in `index.html`         |
| Carousel dishes        | `.item` elements and images in `Images/`                   |
| Rotating ring text     | The `textCircle` string in the script at the bottom        |
| Splash logo            | `Images/quickbiteslogo.png`                                |
| Download button link   | The `.download-button` link in `index.html`                |
