# 🛩️ SKYBOUND: GODFALL — The Last Wingman

**A single-file HTML5 Canvas shoot-'em-up campaign, built for the 12th IUT ICT FEST 2026 Game Jam.**

> "The first shot chooses the war. Then every marked kill points to the next connected target."

Made by **Team CompileAndCry** (3 members).

---

## 🎮 Play It

The whole game lives in one file: [`index.html`](./index.html). No build step, no server required.

1. Clone the repo:
   ```bash
   git clone https://github.com/waseefmunir-max/Gamejam-CompileAndCry.git
   ```
2. Open `index.html` directly in a modern browser (Chrome/Edge/Firefox recommended).
3. Fly.

> The game ships with built-in fallback art and audio, so it runs out of the box. If `assets/` (Kenney "Pixel Shmup" CC0 sprites) and `fonts/` are present alongside `index.html`, it will use those instead — otherwise it silently falls back to procedurally drawn visuals.

---

## 📖 About

**SKYBOUND: GODFALL** is a 10-mission arcade dogfighting campaign about Ilyas, a pilot dragged back into a war he thought he'd escaped, and Rael, the friend on the other side of it. It follows a 10-chapter story (**I. → X. THE LAST WINGMAN**) told through in-mission radio chatter, culminating in a final boss fight and a moral choice that decides how the story ends.

Built entirely as a self-contained HTML5 Canvas application — no external engine, no dependencies — with embedded cinematic audio, procedural sprite fallbacks, and a full save system.

---

## ✨ Key Features

- **SKYLINK CATALYST** — the signature hook. Your first shot each encounter chooses a *doctrine* (weapon behavior), and every following marked kill chains into the next connected target, ramping up your firepower the longer you keep the chain alive.
- **10-level story campaign** with unique dialogue, weather, and a hand-built boss roster (Iron Howl, The Butcher, the Executioner, and GODFALL itself).
- **Per-level Challenges** — a full set of gameplay modifiers, one (or more) per level, each with its own name and on-screen callout:

  | Lv | Challenge | What it does |
  |----|-----------|---------------|
  | 1  | *(none)* | Clean run, learn the basics |
  | 2  | **Manual missile aim** | Missiles lose auto-lock — aim them like bullets |
  | 3  | **GHOSTS DON'T MISS** | Enemies flicker invisible but can still hit you; boss fight also loses missile lock |
  | 4  | **NOWHERE IS SAFE** | Random danger zones cover ~25% of the map — staying in one kills you in ~2.5s |
  | 5  | **YOUR HANDS BETRAY YOU** | Horizontal steering is inverted |
  | 6  | **HELL CHANGES ITS MIND** | Boss fight alternates Lv4/Lv5's challenges every 6s; both active at once in the desperate phase |
  | 7  | **THUNDER KNOWS YOUR NAME** | Telegraphed zones get struck by lightning shortly after |
  | 8  | **THE VOID WON'T LET GO** | Your aircraft keeps drifting after you let go of the stick |
  | 9  | **THE SENTENCE IS DEATH** | A periodic execution-lock reticle targets you — break it or dodge it |
  | 10 | **GOD HATES FAIR FIGHTS** | Two random challenges from the whole pool run simultaneously and rotate throughout the fight against a corrupted, blackened mirror of your own aircraft |

- **Difficulty tiers**: ROOKIE / VETERAN / EXTREME, each reshaping distance, obstacle density, enemy aggression, and weather.
- **Baby Mode** — an accessibility toggle in More Settings that disables *only* the level challenges above; story, enemies, and progression stay fully active. No code required.
- **GOD MODE** — a hidden authorization-code menu (invulnerability + 10× damage). Runs completed with it active are flagged as cheated and don't count toward progress.
- **Rebindable controls**, multiple save slots, a reactive weather/difficulty music matrix, and a full HUD (SKYLINK chain meter, chapter radio log, boss phase callouts).

---

## 🎯 Controls

| Action | Default Keys |
|---|---|
| Steer left | `←` / `A` |
| Steer right | `→` / `D` |
| *(all bindings are remappable in-game via Settings)* | |

---

## 🛠️ Tech Stack

- **HTML5 Canvas** + vanilla JavaScript — single file, zero dependencies
- Embedded cinematic audio (base64-encoded, no external audio files needed)
- Procedural sprite fallback system (drops in cleanly if `Kenney Pixel Shmup` CC0 assets aren't present)

---

## 📂 Project Structure

```
index.html        # the entire game — canvas, engine, audio, UI, story data
assets/           # (optional) Kenney "Pixel Shmup" CC0 sprites, if provided
fonts/            # (optional) Oxanium / Share Tech Mono / Black Ops One
```

---

## 👥 Team

**Compile & Cry** — 3 members, built for the 12th IUT ICT FEST 2026 Game Jam.

## 🏆 Event

- **Jam:** [12th IUT ICT FEST 2026 GameJam](https://itch.io/jam/12th-iut-ict-fest-2026-gamejam)
- **Event site:** [iutictfest26.tech/gamejam](https://iutictfest26.tech/gamejam)
- **Rulebook:** [iutictfest26.tech/gamejam/rulebook](https://iutictfest26.tech/gamejam/rulebook)
- **Organized by:** Islamic University of Technology (IUT), OIC

---

## 📜 License

Created for the ICT FEST 2026 Game Jam. Licensing details to be finalized after the competition concludes.
