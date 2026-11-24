# Cartloom — Minimalist Editorial E-Commerce Experience

[![Deploy static content to Pages](https://github.com/gauravruns/Cartloom/actions/workflows/static.yml/badge.svg)](https://github.com/gauravruns/Cartloom/actions/workflows/static.yml)
[![Live Demo](https://img.shields.io/badge/Demo-GitHub%20Pages-0a0a0a?style=flat&logo=github)](https://gauravruns.github.io/Cartloom/)
[![License: MIT](https://img.shields.io/badge/License-MIT-4a7c59.svg)](LICENSE)

**Cartloom** (branded in-app as **Stuff™**) is an editorial e-commerce storefront engineered for curated lifestyle objects, bespoke lighting, and design-led apparel. Built with a focus on editorial minimalism and fluid motion, it blends real-time 3D WebGL graphics with tactile micro-interactions.

🌐 **Live Showcase**: [https://gauravruns.github.io/Cartloom/](https://gauravruns.github.io/Cartloom/)

---

## ✨ Design Philosophy & Aesthetic

- **Editorial Layout**: High-contrast typography pairing geometric display headers (**Syne**), timeless editorial serif accents (**Instrument Serif**), and technical monospaced labels (**DM Mono**).
- **Curated Palette**: Deep charcoal ink (`#0a0a0a`), warm cream canvas (`#f8f6f1` / `#f2ede4`), sage green (`#4a7c59`), and warm amber highlights (`#f5c842`).
- **Tactile Motion**: Custom spring and cubic-bezier easing curves (`cubic-bezier(0.16, 1, 0.3, 1)`) deliver snappy, Apple-grade responsiveness across every hover, modal, and drawer transition.

---

## 🚀 Core Features

### 1. Interactive 3D WebGL Hero Canvas
- Powered by **Three.js** (`r128`).
- Procedurally generated 3D geometry (architectural domes, cones, pins, vases, and clockwork artifacts) rendered directly in the browser with realistic specular shading, dynamic ambient lighting, and interactive mouse parallax.

### 2. 3D Perspective Card Tilt
- Product showcase cards feature smooth mathematical 3D perspective tilting calculated from mouse cursor coordinates, complete with glare/sheen gradients.

### 3. Reactive Slide-out Cart Drawer
- Seamless fly-out drawer with zero layout shift.
- Real-time cart state management: increment/decrement quantities, instant item removal, and auto-updating badge counters.
- **Fly-to-Cart Animation**: Visual particle/clone trajectory connecting product action triggers directly to the header cart trigger.
- Automatic currency calculation in Indian Rupee (`₹`).

### 4. Product Quick-View Modal
- Detailed product inspection overlay with high-resolution imagery, verified buyer review summaries, categorized badges, and granular quantity controls.

### 5. Custom Kinetic Cursor
- Smooth trailing cursor follower with dynamic scale-up, blending modes, and magnetic attraction states when hovering over interactive elements.

### 6. Full Responsiveness & Mobile Drawer
- Adaptive layout tailored for ultra-wide displays down to mobile viewports.
- Native touch-friendly mobile slide navigation overlay.

### 7. Ancillary Commerce Modules
- Dynamic category filtering across Lighting, Objects, Apparel, and Electronics.
- One-tap Wishlist toggling with micro-animations.
- Auto-scrolling Testimonials marquee.
- Animated stat counters tracking satisfied collectors, handmade runs, and sustainability metrics.
- Interactive Newsletter subscription form with real-time feedback toast notifications.

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Structure** | HTML5 Semantic Architecture | Accessible layout, SEO meta tags, and OpenGraph tags |
| **Styling** | Modern Vanilla CSS3 | Custom properties, CSS Grid, Flexbox, hardware-accelerated animations |
| **3D Engine** | Three.js (r128 CDN) | Procedural 3D scene rendering, lighting, and mouse-reactive mesh rotation |
| **Interactivity** | Vanilla JavaScript (ES6+) | Stateful cart engine, modal system, tilt physics, cursor kinetics |
| **Typography** | Google Fonts | `Syne`, `Instrument Serif`, `DM Mono` |
| **CI/CD & Hosting**| GitHub Actions & GitHub Pages | Automated build and static deployment pipeline |

---

## 📂 Directory Structure

```text
Cartloom/
├── .github/
│   └── workflows/
│       └── static.yml       # GitHub Actions automated deployment to GitHub Pages
├── index.html               # Complete self-contained single-page application (HTML/CSS/JS)
└── README.md                # Project documentation and specifications
```

---

## 🛠️ Local Development

Because Cartloom is built with zero build step dependencies, you can run it immediately with any local HTTP server.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/gauravruns/Cartloom.git
   cd Cartloom
   ```

2. **Launch a local static server:**
   - Using Python:
     ```bash
     python -m http.server 8000
     ```
   - Using Node.js (`npx serve`):
     ```bash
     npx serve .
     ```
   - Or open `index.html` directly in your browser.

3. **View the application:**
   Navigate to `http://localhost:8000` in your browser.

---

## 🚠 Deployment

Deployments are fully automated via GitHub Actions:
1. Any push to the `main` branch triggers `.github/workflows/static.yml`.
2. The repository root is packaged and deployed directly to **GitHub Pages**.
3. The live deployment is served securely over HTTPS at `https://gauravruns.github.io/Cartloom/`.

---

## 👨‍💻 Author

**Gaurav Kumar**
- GitHub: [@gauravruns](https://github.com/gauravruns)

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for details.