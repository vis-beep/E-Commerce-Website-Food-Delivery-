# 🍽️ Badiger's Den — Premium Food Delivery Web App

<div align="center">

![Badiger's Den Banner](https://img.shields.io/badge/BADIGER'S-DEN-C0392B?style=for-the-badge&labelColor=0D0D0D&color=D4AF37)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-D4AF37?style=for-the-badge)

**A fully functional, single-file premium food delivery web application — no frameworks, no dependencies, just pure HTML, CSS & JavaScript.**

[🚀 Live Demo](#) · [📦 Download](#getting-started) · [🐛 Report Bug](../../issues) · [✨ Request Feature](../../issues)

</div>

---

## 📸 Preview

| Login Page | Home / Hero | Menu & Cart |
|:---:|:---:|:---:|
| Split-screen with animated brand panel | Decorated hero with floating cards | Food grid with live cart sidebar |

---

## ✨ Features

- 🔐 **Login & Sign-Up Page** — Dual-tab auth form with Google & Apple social buttons
- 🏠 **Decorative Front Page** — Animated hero, floating cards, dot-grid background, arc rings
- 📂 **Category Filter** — Filter food by Pizza, Burger, Noodles, Sushi, Salads, Desserts, Drinks
- 🛒 **Add to Cart** — Per-item quantity controls (＋/−) with live badge count on navbar
- 📋 **Cart Sidebar** — Slide-in drawer with subtotal, delivery fee, 5% tax, and grand total
- ✅ **Order Placement** — Place order modal with success animation
- 📱 **Responsive Design** — Mobile-friendly layout with media queries
- 🎨 **Luxury Branding** — Crimson + Antique Gold palette, Cormorant Garamond + Bebas Neue fonts
- 🍞 **Toast Notifications** — Animated bottom toast for cart and coupon actions
- 🎟️ **Promo Banner** — 50% off first-order coupon section (code: `DEN50`)

---

## 🗂️ Project Structure

```
badigers-den/
│
├── badigers-den.html       # 🔥 Entire app — single self-contained file
└── README.md               # 📖 This file
```

> **Everything lives in one HTML file** — HTML structure, CSS styles, and JavaScript logic are all bundled together for maximum portability.

---

## 🚀 Getting Started

### Option 1 — Open directly in browser
```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/badigers-den.git

# Navigate into the folder
cd badigers-den

# Open in your default browser
open badigers-den.html        # macOS
start badigers-den.html       # Windows
xdg-open badigers-den.html    # Linux
```

### Option 2 — Serve locally (optional)
```bash
# Using Python (no install required)
python3 -m http.server 8000

# Then visit:
# http://localhost:8000/badigers-den.html
```

### Option 3 — Deploy to GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your site will be live at `https://YOUR_USERNAME.github.io/badigers-den/badigers-den.html`

---

## 🧭 How to Use the App

| Step | Action |
|------|--------|
| 1 | Open `badigers-den.html` in any modern browser |
| 2 | Click **"Enter the Den"** on the login screen (pre-filled credentials) |
| 3 | Browse the menu or filter by category using the pill buttons |
| 4 | Click **"Add to Order"** on any dish — quantity controls appear |
| 5 | Click the 🛒 cart icon in the navbar to open the cart sidebar |
| 6 | Review your order, see live totals, then click **"Place Order"** |
| 7 | Get a success confirmation modal 🎉 |

---

## 🎨 Design System

### Color Palette
| Token | Hex | Usage |
|-------|-----|-------|
| `--crimson` | `#C0392B` | Primary CTAs, accents |
| `--ember` | `#E74C3C` | Hover states |
| `--gold` | `#D4AF37` | Brand accent, borders |
| `--gold2` | `#F0C040` | Hover gold |
| `--ink` | `#0D0D0D` | Dark text |
| `--parchment` | `#FAF5EC` | Page background |
| `--tan` | `#E8DCC8` | Subtle fills |
| `--muted` | `#8A7968` | Secondary text |

### Typography
| Font | Role |
|------|------|
| **Cormorant Garamond** | Headings, food names, prices — elegant serif |
| **Bebas Neue** | Brand name tiers ("BADIGER'S", "DEN") — bold display |
| **DM Sans** | Body text, buttons, labels — clean sans-serif |

---

## 🍔 Menu Data

The app ships with **8 sample dishes** across 7 categories. To add or modify dishes, edit the `foods` array in the `<script>` section of `badigers-den.html`:

```javascript
const foods = [
  {
    id: 9,
    name: 'Your Dish Name',
    desc: 'Short description of the dish.',
    price: 299,           // Price in ₹
    emoji: '🌮',          // Display emoji
    tag: 'new',           // 'best' | 'new' | 'veg'
    tagLabel: 'New',      // Label shown on card
    cat: 'burger',        // Category filter key
    color: '#FFE8D0',     // Card background tint
    rating: 4.7,
    reviews: 500
  },
  // ...
];
```

---

## 📱 Responsive Breakpoints

| Breakpoint | Behaviour |
|-----------|-----------|
| `> 768px` | Full two-column hero, visible nav links, side-by-side layout |
| `≤ 768px` | Single column hero, collapsed nav, full-width cart drawer, stacked footer |

---

## 🛠️ Tech Stack

| Technology | Purpose |
|-----------|---------|
| HTML5 | Structure & semantic markup |
| CSS3 | Styling, animations, CSS variables, Grid & Flexbox |
| Vanilla JavaScript | Cart logic, DOM rendering, state management |
| Google Fonts API | Cormorant Garamond, Bebas Neue, DM Sans |

**Zero npm packages. Zero frameworks. Zero build steps.**

---

## 🔮 Roadmap / Future Improvements

- [ ] Backend integration (Node.js / Firebase)
- [ ] Real authentication (JWT / OAuth)
- [ ] Payment gateway (Razorpay / Stripe)
- [ ] Order tracking with live map
- [ ] User profile & order history
- [ ] Admin dashboard for menu management
- [ ] PWA support (offline mode + install prompt)
- [ ] Dark mode toggle

---

## 🤝 Contributing

Contributions are welcome! Here's how:

```bash
# 1. Fork the repo
# 2. Create your feature branch
git checkout -b feature/amazing-feature

# 3. Commit your changes
git commit -m "Add amazing feature"

# 4. Push to your branch
git push origin feature/amazing-feature

# 5. Open a Pull Request
```

---

##Delopyed Link
**https://vis-beep.github.io/E-Commerce-Website-Food-Delivery-/Badiger.html**

---



## 👨‍💻 Author

**Vishnu Badiger** — *Built with passion and ☕*

> _"Where every dish is a masterpiece, every meal a memory."_
> — Badiger's Den

---

<div align="center">

⭐ **Star this repo if you found it useful!** ⭐

Made with ❤️ using pure HTML, CSS & JavaScript

</div>
