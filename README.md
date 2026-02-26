# Rainbow Unicorn Quest — Co-op Edition

A side-scrolling platformer built entirely in a single HTML file with HTML5 Canvas. No frameworks, no build step — just open and play.

**Play Co-op:** [https://glen-collab.github.io/coop_unicorn/](https://glen-collab.github.io/coop_unicorn/)

**Play Single Player:** [https://glen-collab.github.io/Unicorn/](https://glen-collab.github.io/Unicorn/)

## The Game

Guide your unicorn through 8 worlds (32 levels) of platforming, pooping on enemies, reviving flowers, and battling bosses. Collect power-ups, transform into different forms, and save the Rainbow Land from the Shadow Queen.

### Controls

| Action | Keyboard | Controller |
|--------|----------|------------|
| Move | Arrow Keys / WASD | D-Pad / Left Stick |
| Jump | Space / Up | A Button |
| Poop | P / Right Shift / X | B Button |
| Shoot Rainbow | F / Left Shift | X Button |
| Pause | Escape | Start |
| Start Game | Enter | Start |

### Worlds

1. **Meadow Valley** — Gnomes, flies, and the Gnome King boss
2. **Williams Lake** — Underwater levels, fish, jellyfish, and the Giant Squid boss
3. **Whisker Woods** — Treetop platforming, birds, and the Hawk boss
4. **Fairy Falls** — Misty waterfalls, cascading platforms, and the Flower boss
5. **Sewer Depths** — Alternating dry/flooded tunnels and the Rat King boss
6. **Around the World** — Multi-zone levels (jungle, desert, pyramid) and the Pharaoh Cat boss
7. **Sky Kingdom** — Cloud/storm/star themes with the Storm Dragon boss
8. **Rainbow Land** — Rainbow/crystal/prismatic themes and the Shadow Queen final boss

### Player Forms

- **Unicorn** — Base form with jump, double jump, triple jump (with wings)
- **Mermicorn** — Mermaid form for underwater agility
- **Kittycorn** — Cat form with boosted double jump
- **Pixicorn** — Fairy form with float ability
- **Mousicorn** — Mouse form, small and quick

### Power-Up System

- **Stars** — Collect 5 for rainbow horn shooter
- **Dead Flowers** — Poop on them to revive (20 = 1UP)
- **Black Flowers** — Poop on them for hay bale (grow big) or 1UP if already big
- **Wing Crystals** — Gain wings for triple jump
- **Form Gems** — Transform into mermicorn/kittycorn/pixicorn/mousicorn

### Audio

Full audio system with:
- 10 background music tracks (per-world + boss + title + game complete)
- 17 WAV sound effects (jump, death, poop, bloom, collect, etc.)
- Per-form synthesized poop sounds (mermaid bubbles, kittycorn squeaks, pixicorn sparkles, mousicorn chirps)
- Music crossfades between levels and states

### World Codes

Beat a world boss to get a save code. Enter codes on the title screen (press C):
- **LAKE** — Start at World 2
- **TREE** — Start at World 3
- **FAIR** — Start at World 4
- **PIPE** — Start at World 5
- **SAND** — Start at World 6
- **STAR** — Start at World 7
- **MOON** — Start at World 8

## Project Structure

```
index.html          — The entire game (single file, ~11000 lines)
sprites/            — 49 PNG sprite sheets (player forms, enemies, bosses)
sounds/             — 31 audio files (17 WAV sfx + 14 MP3 music)
```

## Tech

- Pure HTML5 Canvas + JavaScript — no dependencies
- WebAudio API for all sound (oscillator fallbacks if files fail to load)
- Gamepad API for controller support
- Seeded RNG for deterministic level generation
- Procedural drawing fallbacks for all sprites
