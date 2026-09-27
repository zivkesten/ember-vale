# Ember Vale

An original, one-level browser beat-'em-up inspired by the broad conventions of 1990s side-scrolling arcade games. It does not include any SEGA assets, character names, recordings, music, or code from the unlicensed lrusso/GoldenAxe repository.

## Play

Open `index.html` in a browser or on GitHub Pages. On mobile, use the on-screen directional pad and Strike, Jump, Magic buttons. In a desktop browser, use arrows/WASD, J, K, L, P.

Four waves, three lives, score, food and potion pickups, chained attacks, knockback, depth-lane enemy AI, jump arcs, and area magic. Before play, choose one of three original archetypes: barbarian, dwarf, or amazon. These are visual choices with the same game balance. Skeletons, raiders, and iron-clad wardens arrive in different mixes by wave. The scenery uses original canvas-drawn pixel geometry, sunset mountains, trees, stone columns, road stones, and a beacon gate. Portrait shows the game and controls stacked; landscape overlays controls on the full-height game. No network access, sign-in, analytics, or audio. This is not a one-to-one reconstruction of Golden Axe.

## Source note

The reference at https://github.com/lrusso/GoldenAxe is a Phaser-based JavaScript demo. It bundles images, sounds, and music with an educational-use disclaimer and publishes no explicit license. None of its files are included here.

## Decisions / handoff

- 2026-09-27: Use original canvas geometry and original name due to missing license and SEGA-owned media in the reference.
- 2026-09-27: Static single-file deployment to GitHub Pages for phone access. No backend or data is necessary.
- Verify on a physical Pixel for ergonomics before describing it as device-tested; desktop mobile emulation is a separate check.

## PRD / handoff update, 2026-09-27

- Direction: a warmer 1980s fantasy arcade cabinet feel without tracing or importing any Golden Axe sprite, name, logo, sound, or code. Hand-drawn hard-edged canvas geometry keeps the work original.
- Presentation: three selectable hero silhouettes, angular weapon swings and broad slash arcs, bone and armored enemy silhouettes, more particles on hits, visible potion bottles, richer layered ruins and road. Existing keyboard and touch bindings stay unchanged.
- Design scope: hero choice is cosmetic, combat math remains shared; avoids implying separately tuned classes. The stage stays four waves and ends at the beacon.
- Test checklist: desktop launch, movement, chained strikes, jump, magic, pickup, pause/resume; 390 px portrait and landscape with buttons visible and responsive. Physical Android device has not been tested.
