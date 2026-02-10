# 🌍 BreathingEarth

**An interactive climate intervention simulation** — watch Earth's atmosphere degrade in real time, then deploy plasma reactors and direct-air-capture systems to reverse the damage.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

---

## Demo

Open `index.html` in any modern browser — no build step or server required.

## How It Works

The simulation runs through three phases:

| Phase | What Happens |
|---|---|
| **Degradation** | Years tick from 2029 → 2047. Greenhouse gas levels (SF₆, HFCs, CH₄, CO₂, N₂O, CFC-12) rise and temperature anomaly climbs from +2.13 °C toward +3.82 °C. |
| **Intervention** | Hit *Deploy Solution* to activate plasma decomposition reactors and DAC (Direct Air Capture) units. Gas bars animate down in three recovery stages. |
| **Recovery** | Temperature drops to +1.62 °C, gas levels stabilize, and the background video switches to a healthy Earth. Reset to run again. |

A full-bleed background video (`bad.mp4` / `good.mp4`) reflects the current state of the planet while a frosted-glass dashboard panel displays live telemetry.

## Project Structure

```
BreathingEarth/
├── index.html   — Full app (HTML + CSS + JS, single file)
├── bad.mp4      — Degradation-state Earth video
├── good.mp4     — Recovery-state Earth video
└── README.md
```

## Features

- **Zero dependencies** — pure HTML / CSS / JS, no frameworks  
- **Staggered page-load animation** with CSS keyframes  
- **Backdrop-filter glass panel** with SVG grain texture overlay  
- **Responsive layout** — stacks vertically on small screens  
- **Accessible** — focus-visible states, high-contrast status badges, semantic markup  
- **CSS custom properties** for full theme control  

## Usage

```bash
# Clone the repo
git clone https://github.com/SC136/BreathingEarth.git

# Open in browser
cd BreathingEarth
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or use a local server:

```bash
npx serve .
```

## Typography & Design

| Role | Font |
|---|---|
| Display (year counter, title) | DM Serif Display |
| UI / body | Space Grotesk |
| Data / monospace | Space Mono |

Fonts are loaded from Google Fonts. The colour system uses CSS variables defined in `:root` — override them to re-theme the dashboard.

## License

[MIT](LICENSE)
