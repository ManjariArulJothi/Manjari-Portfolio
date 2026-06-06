# Manjari-Portfolio
# 🌐 Manjari PA — Developer Portfolio

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Responsive](https://img.shields.io/badge/Responsive-Yes-brightgreen?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)

> A dark-themed, animated personal portfolio built with pure HTML, CSS, and Vanilla JS — no frameworks, no dependencies.

**🔗 Live:** [manjariarulJothi.github.io](https://ManjariArulJothi.github.io)

---

## ✨ Preview

```
┌──────────────────────────────────────────────────────┐
│  nav: Manjari PA    About  Skills  Projects  Hire Me  │
├──────────────────────────────────────────────────────┤
│                                                        │
│   • AVAILABLE FOR INTERNSHIPS                         │
│                                                        │
│   Manjari                   CGPA     250+             │
│   PA.          ──────────   9.3   Problems Solved     │
│                                                        │
│   [ View Projects ↓ ]  [ Get In Touch → ]             │
│                                                        │
├──────────────────────────────────────────────────────┤
│  About  │  Skills  │  Projects  │  Achievements  │ Contact │
└──────────────────────────────────────────────────────┘
```

---

## 🚀 Features

- **Custom Cursor** — Glowing dot + lagging ring cursor with hover scale effects
- **Scroll Reveal Animations** — Sections animate in as you scroll using IntersectionObserver
- **Active Nav Highlight** — Navbar link highlights based on current scroll position
- **Noise Texture Overlay** — Subtle grain overlay for depth and atmosphere
- **Grid Background** — Animated radial-masked grid in the hero section
- **Responsive Design** — Fluid `clamp()` typography scales from mobile to ultrawide
- **Fluid Typography** — All font sizes use `clamp(min, vw, max)` for perfect scaling
- **Zero Dependencies** — Pure HTML + CSS + Vanilla JS, no npm, no build step
- **Single File** — Entire portfolio in one `index.html` for easy hosting

---

## 🎨 Design System

| Token       | Value                        | Usage                     |
|-------------|------------------------------|---------------------------|
| `--bg`      | `#0a0a0f`                    | Page background           |
| `--bg2`     | `#111118`                    | Alternate section bg      |
| `--surface` | `#16161f`                    | Cards and panels          |
| `--accent`  | `#7ee8a2`                    | Primary green accent      |
| `--accent2` | `#38bdf8`                    | Sky blue accent           |
| `--accent3` | `#f472b6`                    | Pink accent               |
| `--text`    | `#e8e8f0`                    | Primary text              |
| `--muted`   | `#6b6b80`                    | Secondary / dimmed text   |
| Display Font| `Syne` (800 weight)          | Headings, name, titles    |
| Body Font   | `DM Sans` (300–500 weight)   | Paragraphs, labels        |

---

## 📁 File Structure

```
portfolio/
│
├── index.html          # Entire portfolio (HTML + CSS + JS in one file)
└── README.md           # This file
```

> All styles are in a `<style>` block and all scripts in a `<script>` block inside `index.html`.


## ⚙️ Getting Started

### Option 1 — Open Directly (Simplest)

```bash
# Clone the repo
git clone https://github.com/ManjariArulJothi/ManjariArulJothi.github.io.git

# Open in browser
open index.html
# or just double-click index.html
```

### Option 2 — Local Dev Server

```bash
# Using VS Code Live Server extension
# Right-click index.html → "Open with Live Server"

# Or using Python
python3 -m http.server 5500
# Visit http://localhost:5500
```

---

## 🌍 Deployment on GitHub Pages (Free Hosting)

### Step 1 — Create the repo

Create a GitHub repository named exactly:
```
ManjariArulJothi.github.io
```

### Step 2 — Push the file

```bash
git init
git add index.html README.md
git commit -m "Initial portfolio"
git remote add origin https://github.com/ManjariArulJothi/ManjariArulJothi.github.io.git
git branch -M main
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** → **Pages**
3. Under Source → select **main** branch → **/ (root)**
4. Click **Save**

*(takes ~2 minutes to go live)*

---

## 🎯 Customization Guide

### Update your stats
Find the hero stats section in `index.html` and edit the numbers:
```html
<div class="h-stat-num">9.3</div>   <!-- Your CGPA -->
<div class="h-stat-num">250+</div>  <!-- Problems solved -->
<div class="h-stat-num">3+</div>    <!-- Projects count -->
<div class="h-stat-num">4</div>     <!-- Certifications -->
```

### Add a new project
Copy one `.project-card` block and update the title, stack, bullets, and GitHub link:
```html
<div class="project-card reveal">
  <div>
    <div class="proj-header">
      <div class="proj-title">Your Project Name</div>
      <span class="lp-badge green">Your Badge</span>
    </div>
    <div class="proj-stack">
      <span>Spring Boot</span><span>MySQL</span>
    </div>
    <ul class="proj-bullets">
      <li>What you built and <strong>key metric</strong></li>
    </ul>
  </div>
  <div class="proj-meta-col">
    <div class="proj-year">2026</div>
    <a href="https://github.com/..." class="proj-link">GitHub ↗</a>
  </div>
</div>
```

### Change accent color
Edit the CSS variable at the top of the `<style>` block:
```css
:root {
  --accent: #7ee8a2;   /* Change this to any color */
}
```

---

## 📱 Responsive Breakpoints

| Viewport     | Behavior                                       |
|--------------|------------------------------------------------|
| `> 1024px`   | Full layout, two-column about, all nav links   |
| `768–1024px` | Slightly reduced spacing, same layout          |
| `< 768px`    | Single column, nav links hidden, no cursor     |

All font sizes use `clamp(min, vw, max)` — they scale automatically between breakpoints without media queries.

---

## ⚡ Performance

- **No external JS libraries** — zero JS bundle weight
- **Google Fonts** — only 2 font families loaded (Syne + DM Sans)
- **CSS animations** — all effects are GPU-accelerated (`transform`, `opacity`)
- **IntersectionObserver** — scroll reveals are lazy, no scroll event listeners
- **Single HTTP request** for the main file

---

## 🔮 Planned Improvements

- [ ] Add dark/light theme toggle
- [ ] Connect contact form to EmailJS
- [ ] Add project demo GIFs/screenshots
- [ ] Add blog/articles section
- [ ] PWA support (offline access)

---

## 👩‍💻 Author

**Manjari PA**
- 📧 [manjaripa20@gmail.com](mailto:manjaripa20@gmail.com)
- 🐙 [github.com/ManjariArulJothi](https://github.com/ManjariArulJothi)
- 💼 [linkedin.com/in/ManjariArul](https://linkedin.com/in/ManjariArul)
- 📍 Tiruppur, Tamil Nadu

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> B.Tech IT Student @ Dr. Mahalingam College of Engineering and Technology (2024–2028)  
> Building backends that scale. ⚡
