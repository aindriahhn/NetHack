# NHMRP — Nethack Mobile Restoration Project

A single-file, mobile-first roguelike in the shape of NetHack, written in
plain HTML/JavaScript. Open the game file in a browser — no install, no
build step. A passion project, not a commercial release.

## Canonical build

**`NHMRP_1.02__yendor_1.html` is the canonical build.**

- Descend to depth 10, find the Amulet of Yendor, and climb back out.
  There are no stairs down past depth 10; once the Amulet is carried,
  stairways up (`<`) appear and climbing from depth 1 wins the game.
- Creature remains: monsters (except slime) drop remains that can be
  eaten for per-creature effects or thrown at a target for the same effect.
- Dunking: stand on a fountain or sink, use the Dunk button, and tap an
  inventory item. Effects are specific per item — torches go out, scrolls
  go blank, weapons quench, rings slip down sink drains.
- 4 roles (Barbarian, Wizard, Rogue, Archer), 11 monster types, shops,
  fountains, sinks, altars, vaults, traps, gas and fire, pets, save/load,
  and a dead-runs record.

## Other files in this repo (archived, not canonical)

- `NetHack.html` — the previous line (the 1.01 build's GitHub step).
- `NHMRP.html` — a divergent branch of the same game, not merged.
- `index.html` and `Nethack-beta` — older siblings.
- `Easy-Nethack` — an early sketch.

These are kept for history. New work goes into the canonical file above,
as a sibling build, with the originals left untouched.

## Playing

Open `NHMRP_1.02__yendor_1.html` in a browser, tap New Game, pick a role,
and use the on-screen controls. Keyboard play works too. Progress saves
to the browser's local storage under the game's own save key.
