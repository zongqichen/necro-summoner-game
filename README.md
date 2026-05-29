# Necro Summoner

A Diablo-2-flavoured necromancer auto-combat prototype. Move, raise named skeletons, watch them permadeath. Pure HTML5 Canvas + vanilla JS, zero build step.

**▶ Play:** https://zongqichen.github.io/necro-summoner-game/
**📦 Source:** https://github.com/zongqichen/necro-summoner-game

## Status

Pre-alpha (v0.2). The prototype tests one core loop question: _does an auto-summoned, named, mortal minion create emotional attachment in 5 minutes?_

## Concept

- **Theme:** necromancer + undead legion
- **Core loop:** kill enemies → gain XP → level up → pick perks (incl. unlock new minion classes) → survive 5 minutes → defeat the boss
- **Player input:** movement only — auto-attack and auto-summon happen on their own
- **Each minion is a person:** random first name, title, and one-line backstory; their permadeath is logged
- **Single-screen arena:** enemies enter from any of the four edges, difficulty ramps every minute, BOSS at 5:00

## Features (v0.2)

- 6 summonable minion classes: warrior, archer, mage, knight, assassin, berserker
- 9 enemy kinds (incl. one ranged caster) + boss
- Identity pool: 30 first names × 25 titles × 22 backstories per language
- EN / 中文 toggle (in-game side panel; persists in localStorage)
- Mobile support: drag-anywhere virtual joystick + responsive layout
- Zero dependencies, ~7 MB total, served as a static site

## Repo layout

```
prototype/index.html     The playable game (single file, vanilla JS)
index.html               Landing page (linked to from GitHub Pages)
public/                  Slim sprite/tileset bundle used by the game
docs/
  competitor-research.md  Genre survey
  concept.md              Gameplay design notes
  design-decisions.md     ADR-style decision log
SECURITY.md              Vulnerability reporting policy
LICENSE-ART.md           CC-BY-SA 3.0 attribution for art
memory/                  Claude Code project memory
```

## Controls

- **Desktop:** WASD / arrow keys to move · Space to pause · R to restart
- **Mobile:** drag anywhere on the play area to move

## Art credits

Skeleton and zombie body sprites from the Liberated Pixel Cup (LPC) project — CC-BY-SA 3.0.
Dungeon tileset from flare-game — CC-BY-SA 3.0.
See [LICENSE-ART.md](./LICENSE-ART.md) for the full attribution list.

## Security

See [SECURITY.md](./SECURITY.md) for private vulnerability reporting.
