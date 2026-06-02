<div align="center">

# Snowfall

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?style=flat-square)](https://soumendrak.github.io/snowfall/)
[![MIT License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-%23E34F26?style=flat-square&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![Zero Dependencies](https://img.shields.io/badge/dependencies-0-success?style=flat-square)](https://www.w3.org/TR/html52/)

<!-- Inline SVG logo -->
<svg width="140" height="140" viewBox="0 0 140 140" xmlns="http://www.w3.org/2000/svg">
<rect width="140" height="140" rx="24" fill="#0a0a14"/>
  <circle cx="30" cy="30" r="3" fill="#ffffff" opacity="0.8"/>
  <circle cx="80" cy="22" r="2" fill="#ffffff" opacity="0.6"/>
  <circle cx="50" cy="45" r="4" fill="#ffffff" opacity="0.7"/>
  <circle cx="110" cy="35" r="2.5" fill="#ffffff" opacity="0.5"/>
  <circle cx="25" cy="60" r="3.5" fill="#ffffff" opacity="0.6"/>
  <circle cx="70" cy="55" r="2" fill="#ffffff" opacity="0.4"/>
  <circle cx="95" cy="70" r="3" fill="#ffffff" opacity="0.7"/>
  <circle cx="45" cy="80" r="2.5" fill="#ffffff" opacity="0.5"/>
  <circle cx="115" cy="55" r="2" fill="#ffffff" opacity="0.6"/>
  <circle cx="60" cy="90" r="3" fill="#ffffff" opacity="0.4"/>
  <circle cx="35" cy="100" r="2" fill="#ffffff" opacity="0.5"/>
  <circle cx="100" cy="95" r="3.5" fill="#ffffff" opacity="0.6"/>
  <text x="70" y="128" text-anchor="middle" font-family="sans-serif" font-size="8" fill="#8a8a9a">click to add wind</text>
</svg>

**A falling snow particle system with wind control and seasonal colour modes.**

**Live:** [https://soumendrak.github.io/snowfall/](https://soumendrak.github.io/snowfall/)

</div>

---

## Features

- 100-300 snowflakes falling with individual size and speed
- Sliders: flake count (50-500), speed, wind intensity
- Click anywhere to add wind bursts that drift particles
- Seasonal colour modes: Winter (white/blue), Spring (green/pink), Random
- Particles sway side to side for realistic motion
- Responsive — fills the full viewport
- Frame-rate independent movement using delta time
- Dark theme with orange accent (#ff6b35)

## How It Works

Each snowflake is an object with x, y, speed, size, opacity, and sway offset. On each frame, `y += speed × dt`, `x += wind × dt + sin(sway) × 0.5`. Wind is a global value adjustable via slider or click. When a flake falls below the viewport, it wraps around to the top. The particle count is dynamically adjustable without recreating the array.

## Usage

1. Open `https://soumendrak.github.io/snowfall/` in any browser.
2. No build step, no installation, no server required.
3. Deploy anywhere — GitHub Pages, Netlify, or any static host.

```bash
git clone https://github.com/soumendrak/snowfall.git
# Open index.html directly
```

## License

Licensed under the [MIT License](LICENSE).

---

<p align="center"><sub>Built with ❤️ and zero dependencies</sub></p>
