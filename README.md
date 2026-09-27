# Ember Vale

An original pixel-art arcade brawler for the browser, built in the spirit of late-1980s side-scrolling fantasy beat-'em-ups. All artwork is hand-drawn in code: no SEGA assets, sprites, names, audio, or code, and nothing from the unlicensed lrusso/GoldenAxe repository.

## Play

Live at https://zivkesten.github.io/ember-vale/ (single `index.html`, served from `main` root via GitHub Pages).

- **Touch**: directional pad, Strike, Jump, Magic. Double-tap left/right to dash.
- **Keyboard**: arrows/WASD to move, J strike, K jump, L magic, P pause. Double-tap a direction to dash.

## The game

Pick one of three heroes - barbarian, dwarf, or amazon - and fight through four side-scrolling stages: the Old Road, the Ruined Village, the Giant Bridge, and the Castle Gate, ending with the boss Warlord Brann.

- Three-hit combos, dash attacks, jump attacks, and throws; enemies can be knocked down and juggled.
- Depth movement: walk up and down the lane, not just left/right.
- Club thugs in several colors, skeletons that rise out of the ground, and armored knights that block frontal hits.
- Rideable beasts: knock the rider off a cockatrice or dragon and mount it; the dragon breathes fire.
- Small thieves dart in and drop magic pots and meat when smacked.
- Leveled magic: pots you collect set the spell level. Barbarian calls fire pillars, dwarf calls lightning, amazon calls a dragon flyby. More pots, bigger spell.
- Arcade HUD: stage number, magic pots + spell level, score, hero portrait with ten life segments, spare-life heads, CREDIT 1, and a red boss bar.
- Title, hero select, stage intro cards, game over, and victory screens. Chiptune-style WebAudio effects.

## Source note

The reference at https://github.com/lrusso/GoldenAxe is a Phaser demo that bundles images, sounds, and music with an educational-use disclaimer and no explicit license. None of its files, and no SEGA material, are included here. Every sprite in Ember Vale is an original part-drawn pixel composition rendered at 320x180 and scaled 3x.

## Decisions / handoff

- 2026-09-27 (round 2): Full rebuild as a pixel-art arcade brawler after the blocky-vector first pass missed the target feel. Hand-drawn parts per character with paper-doll frames (walk, attack, dash, cast, hurt, sit, knockdown). Verified live at 390x844 portrait and 844x390 landscape against original arcade reference screenshots (reference only, never copied).
- 2026-09-27 (round 1): Original canvas geometry and original name because the reference lacks a license and contains SEGA-owned media. Static single-file deployment for phone access.
- Verify on a physical phone before describing the game as device-tested; desktop emulation is a separate check.
