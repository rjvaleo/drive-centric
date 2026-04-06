# RJ Valeo — TPM Pitch · DriveCentric

![Built With](https://img.shields.io/badge/built_with-Vanilla_HTML%2FCSS%2FJS-0f172a?style=flat-square&logo=html5&logoColor=white)
![No Dependencies](https://img.shields.io/badge/dependencies-zero-19c29a?style=flat-square)
![No Build Step](https://img.shields.io/badge/build_step-none-624ba1?style=flat-square)
![GitHub Pages](https://img.shields.io/badge/deployed-GitHub_Pages-222?style=flat-square&logo=github&logoColor=white)
![License](https://img.shields.io/badge/license-personal-lightgrey?style=flat-square)
![File Size](https://img.shields.io/badge/single_file-~2400_lines-19c29a?style=flat-square)

A single-file, zero-dependency interactive pitch page built to apply for the **Technical Project Manager** role at [DriveCentric](https://drivecentric.com). Designed, coded, and deployed by **Richard J. Valeo, CSM** — the TPM who reads the diff.

---

## Live Site

> **[rjvaleo.github.io/drive-centric](https://rjvaleo.github.io/drive-centric/)**

---

## What's in the file

| Section                | Description                                                                    |
| ---------------------- | ------------------------------------------------------------------------------ |
| `01 — The Signal`      | Expandable audit table mapping every JD requirement to direct evidence         |
| `02 — The Build`       | Scale Sequencer project card with live screenshot                              |
| `03 — Proof of Method` | Three tabbed scenario walkthroughs (scope creep, blocked sprint, partner miss) |
| `04 — The CTO Slide`   | Side-by-side "what you're asking / what I deliver" grid                        |
| `05 — Track Record`    | Six role cards across 20 years of delivery                                     |
| `06 — Day 1 · Day 30`  | Concrete two-column ramp plan                                                  |
| `Closer`               | Contact + links                                                                |

---

## Technical Implementation

### Stack

- **Vanilla HTML5** — semantic, accessible markup
- **CSS3** — custom properties, `clamp()`, `@keyframes`, `backdrop-filter`, CSS Grid, Flexbox
- **Vanilla JavaScript (ES2022)** — no frameworks, no libraries, no bundler
- **Google Fonts** — Montserrat (matching DriveCentric brand), Inter fallback

### Features

- **6-theme selector** — DriveCentric brand, Ultraviolet, Terminal, Afterburner, Gold Operator, Glassmorphism
- `localStorage` theme persistence across page reloads
- Custom animated cursor (dot + ring) with hover expand states
- Scroll-driven progress bar
- IntersectionObserver-based scroll reveal animations
- Expandable proof rows (accordion)
- Tabbed scenario panels
- Aurora CSS animation (Glassmorphism theme)
- Scanline overlay (Terminal theme)
- Fully responsive layout
- Zero external JavaScript dependencies
- Zero build step — open `index.html` in any browser

### CSS Architecture

- All colors, gradients, and fonts live in a single `:root` custom property block
- 6 `[data-theme="x"]` override blocks for full theme switching
- No CSS preprocessor required
- DriveCentric brand palette matched from live site inspection:
  - Primary: `#624ba1` (purple)
  - Teal accent: `#19c29a`
  - Background: `#131416`
  - Panel: `#212426`
  - Font: `Montserrat`

---

## File Structure

```
drive-centric/
├── index.html          # Entire app — single file, zero dependencies
├── images/
│   └── scale-sequencer.png   # Scale Sequencer app screenshot
└── README.md
```

---

## Deployment

Deployed to GitHub Pages from the `main` branch root. No CI/CD required — the file is its own artifact.

```bash
git add .
git commit -m "deploy"
git push origin main
```

---

## About the Author

**Richard J. Valeo, CSM**
Georgetown, CO · Remote (U.S.)
[rjvaleo@gmail.com](mailto:rjvaleo@gmail.com) · [917-664-1750](tel:9176641750)
[LinkedIn](https://www.linkedin.com/in/rjvaleo) · [GitHub](https://github.com/rjvaleo) · [Portfolio](https://rjvaleo.github.io/rj-polymath-site/)

20 years of software delivery. 12 of Agile leadership. Active GitHub practice with production-deployed code. This page is the evidence.
