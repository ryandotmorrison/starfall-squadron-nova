# 🚀 Starfall Squadron Nova

A space-shooter + platformer hybrid: pick a hero, pick a ship, and fight across
4 worlds with scoring, combos, power-ups, and multi-phase bosses.

## 🌟 Credit where it's due

**Original game by Ronan** — this project started as Ronan's Phaser space
shooter (hosted at `battle-ship-mu-ashen.vercel.app`). The **Nova Edition** is
an upleveled homage built from his game in October 2026: 4 worlds, 4 heroes,
3 ships, and a full hub with unlocks — but the starship at the heart of it is
Ronan's. Thank you, Ronan!

## 🎮 How to play

Open the game in a browser (or install it — see below) and click / tap to start.

**Keyboard**
- **Arrows / WASD** — move & fly
- **Space** — jump
- **X** — fire
- **Z** — interact
- **B** — bomb
- **P** — pause
- **M** — mute

**Touch (phones & tablets)**
- **Left side** — floating joystick to move
- **Right side** — FIR (fire), JMP (jump), ACT (interact), BMW (bomb)

Clear all hostiles in each wave to advance. Beat all 4 stages to finish the game!

## 📦 What's in this repo

The whole game is **one file**: `index.html` (HTML + CSS + JavaScript, no
build step, no dependencies). The extra files turn it into an installable
phone/tablet app (a PWA):

| File | What it is |
|---|---|
| `index.html` | The entire game — this is the file you edit |
| `manifest.json` | App name, colors, and home-screen icons |
| `sw.js` | Service worker — makes the game work offline after the first visit |
| `icons/` | App icons (180 / 192 / 512 px) |

## 🤝 How to collaborate

Ronan is a collaborator on this repo — you can both edit the game!

1. **Edit `index.html`** — that's the whole game. Keep it a single file (no
   new files needed for game code; art and sound are generated in code).
2. **Test by just opening it** — double-click `index.html`, or run a tiny
   local server: `python3 -m http.server` and visit `http://localhost:8000`.
3. **Commit + push** to the `main` branch — the live game updates automatically
   a minute or two later.
4. **Tips**: small changes first (colors, speeds, enemy counts), play-test
   every change, and don't break the hub — the START MISSION button is sacred. 😄

Ideas if you want a mission: new enemy types, harder wave 6, a 5th world,
co-op mode…

## 📱 Install as an app

On iPhone/iPad: open the live game URL in **Safari** → **Share** →
**Add to Home Screen**. It launches full-screen and works offline after the
first load.

## 🔧 Known issues

- **No sound on iPhone?** Check the **SOUND** button in the hub (bottom-left) —
  it shows 🔇 MUTED when muted, 🔊 SOUND when on. The mute setting is saved on
  the device, so it can survive a reinstall. (A missing-sound report after a
  fresh install is being investigated.)
