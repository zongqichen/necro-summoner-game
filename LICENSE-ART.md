# Art Asset Attribution

The four sprite/tileset images shipped in `/public/` are derivatives of upstream
free art and are redistributed under the original licenses.

## /public/skeleton.png · /public/zombie.png · /public/male_walk.png

Source: **Liberated Pixel Cup (LPC) Universal Spritesheet Character Generator**

- Upstream: https://github.com/LiberatedPixelCup/Universal-LPC-Spritesheet-Character-Generator
- Original LPC contest organized by OpenGameArt.org, Creative Commons, and the Free Software Foundation
- Body sprites (skeleton / zombie / male) authored by **Stephen Challener (Redshrike)**, **Johannes Sjölund (wulax)**, **Manuel Riecke (MrBeast)** and the broader LPC contributor pool.
- License: **CC-BY-SA 3.0** and **GPL-3.0** (dual-licensed by upstream)

## /public/tileset_dungeon.png

Source: **flareteam/flare-game** — `mods/fantasycore/images/tilesets/tileset_dungeon.png`

- Upstream: https://github.com/flareteam/flare-game
- Authored by **Justin Nichol**, **Clint Bellanger**, **Stefan Beller** et al.
- License: **CC-BY-SA 3.0**

---

## What this means for downstream users

Both licenses (CC-BY-SA 3.0 and GPL-3.0) are **share-alike / copyleft**.
Distributing this prototype's art further requires:

1. Attribution to the original authors (this file satisfies it).
2. Any derivative artwork must be released under CC-BY-SA 3.0 (or compatible).

The **game code** in `/prototype/index.html` is authored from scratch and is
**not** derived from FLARE's GPL-3.0 engine code; only the art assets carry
the share-alike obligation.

If commercial / closed-source distribution is later required, these four
images must be replaced with originals or with assets under MIT / CC0 / OGA-BY.
