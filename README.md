# Missile Defense 🚀

A retro arcade-style **Missile Command** tribute — defend 6 cities from incoming nuclear missiles using interceptor explosions. Built as a standalone HTML5 canvas game with desktop + mobile support.

## 🎮 Play

**[Play Now](https://nwfella.github.io/missle-defense/)** — no install, no ads, just click.

## 🕹️ How to Play

| Desktop | Mobile |
|---------|--------|
| Move mouse to aim | Tap to fire at that position |
| Click to launch interceptor | Tap anywhere to fire |

- **3 missile silos** (left, center, right), each with 15 interceptors per wave
- **Interceptors explode** on arrival — the blast destroys any enemy missile in its radius
- **6 cities** to protect — lose them all and it's game over
- **Incoming missiles** travel in ballistic arcs toward your cities
- **Watch for MIRVs** (partially split missiles with a magenta ring) starting wave 3
- **Score bonus** for mid-air interceptions vs. catching missiles at city level

## ✨ Features

- 🌟 Starfield with twinkling parallax
- 💥 Particle explosions, missile trails, neon glow effects
- 🏢 Illuminated city buildings with glowing windows
- 🔊 Web Audio API synthesized sound effects (launch, explosion, game over, wave start)
- 📱 Fully responsive — works on phones, tablets, and desktops
- 🕹️ CRT scanline overlay + vignette for retro feel
- 📊 Ammo indicators per silo, live HUD, wave progression

## 🛠️ Tech

Single-file HTML5 canvas game — no frameworks, no build step, no dependencies.

- **Canvas 2D** — game loop with fixed-timestep accumulator
- **Pointer Events API** — unified mouse + touch input
- **Web Audio API** — synthesized SFX (oscillators + noise buffers)
- **CSS aspect-ratio** — responsive scaling without JS math
- **localStorage** — free (persists best score)

## 🧱 Waves

| Wave | Missiles | Speed Bonus | MIRVs |
|------|----------|-------------|-------|
| 1    | 6        | +0%         | ❌    |
| 2    | 9        | +12%        | ❌    |
| 3    | 12       | +25%        | ✅    |
| N    | 6+3(N-1) | +12% per wave | Increasing chance |

## 🏗️ Project Structure

```
missle-defense/
├── index.html   # The entire game — open in any browser
├── README.md    # This file
└── .nojekyll    # Tells GitHub Pages to serve raw files
```

## 🧪 Running Locally

```bash
# No build step — just open the file
open index.html

# Or serve with any HTTP server
python3 -m http.server 8000
# -> http://localhost:8000
```

## 📜 License

MIT — free to play, share, and remix.
