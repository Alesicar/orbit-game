# Orbit

> Tap to launch satellites. Achieve stable orbits. Create accidental art.

## How to Play

- **Drag to aim** — touch or click and drag to set direction and power, then release to launch
- **Complete one full orbit** around the planet to make a satellite permanent (it turns gold!)
- **Permanent satellites pull new ones** — each stable orbit adds gravitational interference, creating beautiful chaos

## Game Modes

Choose from the menu when the game starts:

- **FREE ORBIT** — Infinite lives, no pressure. Just chill and create orbital art.
- **SURVIVAL** — 5 lives. Each escaped or crashed satellite costs a life. How many orbits can you stabilize?
- **PRECISION** — Exactly 10 launches. No lives system — every shot counts. Maximize permanent orbits with careful aim.
- **DAILY** — A daily challenge with the same random seed for everyone (affects comet timing and star positions). Separate high score. Come back tomorrow and compare!

High scores are tracked separately per mode in localStorage.

## Features

### Comet Events
Every 30–45 seconds, a comet streaks across the screen diagonally — a thin bright line with a fading trail. Purely visual atmosphere. But if a satellite collides with a comet mid-flight, it gets a massive speed boost and leaves a **rainbow trail** for 3 seconds. "SLINGSHOT!" appears in gold. These are screenshot-worthy moments.

### Orbit Streaks
Achieve 3 permanent orbits in a row without any crash or escape to trigger a streak bonus: aurora-like color bands flash across the top of the screen, "+3 STREAK" floats up, and the planet pulses brighter for 5 seconds. The streak counter stays visible during an active streak and resets on any crash or escape.

### Gravitational Lensing
When a satellite passes very close to the planet (within 2× planet radius) without crashing, nearby stars are visually displaced outward — a subtle gravitational lensing effect that rewards observant players.

### Visual Juice
- Non-permanent orbiting satellites have a subtle pulsing glow (radius oscillates 6–10px)
- When a satellite becomes permanent, all other permanent satellites pulse in sequence (wave effect, 100ms delay between each)
- The planet grows slightly (0.5px) with each permanent orbit — by orbit 15, it's noticeably larger, making the game spatially harder

### Screenshot Mode
Double-tap or long-press (1 second) to pause the game and hide all UI. The orbital art fills the whole screen — perfect for screenshotting. Tap again to resume.

### Daily Seed
A daily challenge with a shared random seed (based on date) determines comet timing and initial star positions. Shows "DAILY #XXX" in the menu with a separate high score. Same seed for everyone — compare scores with friends.

### Mobile Haptics
Subtle vibration feedback on supported devices: short buzz on launch, medium on crash, double-pulse on permanent orbit, long on life lost.

## Play

[**Play Orbit**](https://alesicar.github.io/orbit-game/)

## Screenshot

![Orbit gameplay](screenshot.png)

## License

MIT

---

*Built with vibes and vanilla JS on a train in Slovenia*
