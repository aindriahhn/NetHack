# NHMRP — Nethack Mobile Restoration Project

A single-file, mobile-first roguelike in the shape of NetHack, written in
plain HTML/JavaScript. Open the game file in a browser — no install, no
build step. A passion project, not a commercial release.

## Canonical build

**`NHMRP_1.05__sprites_1.html` is the canonical build.**

- Descend to depth 10, find the Amulet of Yendor, and climb back out.
  There are no stairs down past depth 10; once the Amulet is carried,
  stairways up (`<`) appear and climbing from depth 1 wins the game.
- Creature remains: monsters (except slime) drop remains that can be
  eaten for per-creature effects or thrown at a target for the same effect.
- Dunking: stand on a fountain or sink, use the Dunk button, and tap an
  inventory item. Effects are specific per item — torches go out, scrolls
  go blank, weapons quench, rings slip down sink drains.
- Magic, on shared hooks: a spell registry (Healing, Fireball, Frost,
  Teleport, Identification, Haste, Revelation) with role starting spells
  and spellbooks to learn more; wands of fire, frost, and confusion
  alongside striking and teleportation; scrolls of enchant weapon and
  armor (+1, capped at +5, cursed items uncursed instead).
- Sound: a small WebAudio layer in CALORIS's spirit — event sounds for
  hits, deaths, pickups, spells, zaps, stairs, and victory, plus a soft
  ambient note every 6th turn, with a 🔊 toggle.
- Sprites: procedural 16×16 pixel tiles for floors, walls, features,
  monsters, items, traps, and the player, with a 🖼️ toggle — glyphs are
  the default and any unsprited cell falls back to its glyph.
- Mobile play: tap the canvas to move one step toward a tile (in look
  mode, a tap moves the cursor), a larger d-pad, and 44px touch targets.
- 4 roles (Barbarian, Wizard, Rogue, Archer), 11 monster types, shops,
  fountains, sinks, altars, vaults, traps, gas and fire, pets, save/load,
  and a dead-runs record.

## Other files in this repo (archived, not canonical)

- `NHMRP_1.03__magic_1.html` — the previous canonical build.
- `NHMRP_1.02__yendor_1.html` — the build before that.
- `NetHack.html` — the earlier 1.01 line.
- `NHMRP.html` — a divergent branch of the same game, not merged.
- `index.html` and `Nethack-beta` — older siblings.
- `Easy-Nethack` — an early sketch.

These are kept for history. New work goes into the canonical file above,
as a sibling build, with the originals left untouched.

## Playing

Open `NHMRP_1.05__sprites_1.html` in a browser, tap New Game, pick a role,
and use the on-screen controls or tap the canvas to move. Keyboard play
works too. Progress saves to the browser's local storage under the
game's own save key.
