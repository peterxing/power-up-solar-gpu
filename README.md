# ⚡ Power Up! — Solar, Batteries & Home AI Clusters

An interactive educational game built for a **TAFE NSW** course. Learners plan a rooftop **solar & battery install**, build a **home GPU cluster**, then bring it together to **run an AI lab on sunshine** — making real design decisions, sizing real systems, and working safely to Australian standards.

> 🎮 **Play it online:** https://peterxing.github.io/power-up-solar-gpu/

## What's inside

Three modules plus a capstone, each mixing different interactive mechanics:

- **☀️🔋 Solar & Battery Install** — site assessment quiz → interactive system-sizing sliders → sequence the wiring path → standards & compliance quiz
- **🖥️⚡ Home GPU Cluster** — hardware-choice quiz → PSU / power-budget sliders → order the build steps → thermals & safety quiz
- **☀️➜🖥️ Capstone: Run Your AI Lab on Sunshine** — size solar + storage to power the cluster day and night, plus a reflection quiz

Features a running score, progress bar, three unlockable badges, and a graded, printable certificate. Light/dark theme aware. 🌗

## Australian / NSW context

The content is grounded in real NSW conditions and regulations:

- North-facing roofs (Southern Hemisphere), tilt ≈ latitude (~34° for Sydney)
- ~4.2 peak sun hours and a 0.8 performance ratio for sizing estimates
- **AS/NZS 5033** (PV arrays), **4777** (inverter grid connection), **5139** (batteries), **3000** (Wiring Rules)
- CEC / Solar Accreditation Australia (SAA) accreditation & STC eligibility
- 240 V / 10 A circuits, the ~80% continuous-load rule, and when a licensed electrician is legally required

## Running locally

It's a single self-contained HTML file — no build step, no dependencies.

```bash
# just open it
start index.html        # Windows
open index.html         # macOS

# or serve it
npx serve .
```

## Disclaimer

This is an **educational game for learning purposes only** — not a formal qualification. Real solar, battery and electrical work in NSW must be carried out by appropriately licensed and accredited professionals in accordance with current standards and SafeWork NSW requirements.

## License

[MIT](LICENSE)
