# ☀️ Solar Install 3D — Build a Rooftop Solar & Battery System

An interactive **3D installation simulator** built for a **TAFE NSW** course. Learners orbit a real house, choose the correct roof aspect, mount the solar array (avoiding shade), wire the system safely to Australian standards, then switch on the sun and watch a full solar day power the home and charge the battery into the night.

Built with **[Three.js](https://threejs.org/)** — real-time 3D rendering, raycast interaction, dynamic shadows and a day/night cycle, all in a single HTML file.

> 🎮 **Play it online:** https://peterxing.github.io/power-up-solar-gpu/

## How to play

| Control | Action |
| --- | --- |
| 🖱️ **Drag** | Orbit the camera around the house |
| 🔍 **Scroll** | Zoom in / out |
| 👆 **Click** | Select roof faces, place panels, connect components |

## The four installation phases

1. **🧭 Site & Aspect** — Click the roof slope that should carry the panels. In the Southern Hemisphere the sun sits to the north, so the **north-facing** slope wins.
2. **🔆 Mount the Array** — Click roof slots to place 6 panels, mounted flush to the pitch (tilt ≈ latitude). **Avoid the shaded slots** under the tree — shade on one panel drags down the whole string.
3. **🔌 Wire it Safely** — Connect the components in the correct energy-flow order: **PV Array → DC Isolator → Inverter → AC Isolator → Switchboard → Meter/Grid**, with isolators each side of the inverter so it can be switched off safely.
4. **⚡ Commission** — Energise and run a compressed solar day: generation pulses along the wires, the battery banks the daytime surplus, and after sunset the stored energy keeps the home's lights on.

Earn badges (Site Surveyor, Array Ace, Safe Sparky, Night Owl Storage) and finish with a graded practice certificate. Light/dark theme aware. 🌗

## Australian / NSW context

Grounded in real NSW conditions and regulations:

- North-facing roofs (Southern Hemisphere), tilt ≈ latitude (~34° for Sydney)
- ~4.2 peak sun hours used for the generation estimate (~11 kWh/day from a ~2.6 kWp array)
- Shading kills series-string output — a key real-world design constraint
- **AS/NZS 5033** (PV arrays), **4777** (inverter grid connection), **5139** (batteries), **3000** (Wiring Rules)
- Isolate &amp; test before you touch; battery storage shifts daytime sun to night-time load

## Tech notes

- Single self-contained `index.html`. **Three.js** is loaded at runtime from the jsDelivr CDN via an ES-module import map, so an internet connection is required to play.
- No build step. To run locally just serve the folder:

```bash
npx serve .
# then open the printed http://localhost:… URL
```

(Opening the file directly via `file://` also works in most browsers, but serving over HTTP is the most reliable.)

## Disclaimer

This is an **educational simulation for learning purposes only** — not a formal qualification. Real solar, battery and electrical work in NSW must be carried out by appropriately licensed and accredited professionals in accordance with current standards and SafeWork NSW requirements.

## License

[MIT](LICENSE)
