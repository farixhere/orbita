# ORBITA: Virtual Space Explorer

ORBITA is an interactive 3D solar system that runs directly in the browser.
Built for a college science exhibition, it lets visitors fly through space,
explore planets and moons, and learn along the way. No installation is needed.

**Live demo:** https://YOUR-USERNAME.github.io/orbita/

## Features
- The Sun, all 8 planets, 11 moons and the asteroid belt, with procedurally
  generated textures, atmospheres, Saturn's rings and a starfield
- Click a planet or moon, or use the number keys, to fly to it
- Knowledge panels with NASA-based facts, missions and discoveries
- Two-planet comparison with scaled bars
- Spacecraft mode: pilot your own ship through the system
- Missions, a short astronomy quiz, achievements and space-fact cards
  (progress is saved in the browser)
- Cinematic intro, ambient sound, settings and fullscreen
- Exhibition mode: larger interface, a guided auto-tour, and automatic reset
  after 90 seconds without input

## Controls
| Input | Action |
|---|---|
| Drag / scroll | Rotate / zoom the camera |
| Click a body | Travel to it |
| 1–8 | Mercury to Neptune |
| 9 | Asteroid belt |
| 0 / Esc / Home | Overview |
| F | Follow the selected body |
| X | Spacecraft mode (W/S speed, A/D turn, Shift boost) |
| M | Mission Control |
| S | Settings |
| E | Exhibition mode |

## Tech
HTML, CSS and JavaScript (ES modules) with [Three.js](https://threejs.org) 0.170,
loaded from the jsDelivr CDN. There is no build step and no dependencies to install.

## Run locally
Because it uses ES modules, serve it over HTTP instead of double-clicking the file:

    py -m http.server 8000

Then open http://localhost:8000. An internet connection is needed for the Three.js CDN.

## Notes
- The model is stylized: sizes, distances and moon orbits are not to scale.
- Planetary data comes from NASA sources. Moon counts and mission statuses change over time.
- Requires a browser with WebGL (current Chrome, Edge or Firefox).

## Credits
Created by YOUR NAME for YOUR COLLEGE exhibition. Data: NASA Solar System Exploration.
