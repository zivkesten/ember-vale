# Ember Vale PRD and handoff

## Goal
An original browser brawler that feels like a late-1980s fantasy arcade cabinet: side-view stages with depth, mounted beasts, leveled screen-clearing magic, and a chunky pixel HUD. Inspired by the genre's conventions, never a copy: no Golden Axe sprites, names, audio, ROM data, or code.

## Player path
Title screen -> hero select (barbarian, dwarf, amazon) -> stage intro card -> four scrolling stages (Old Road, Ruined Village, Giant Bridge, Castle Gate) -> Warlord Brann boss -> victory. Three lives, 100 HP per life, score, continue-style CREDIT display.

## Combat system
Three-hit strike combo, dash attack (double-tap direction), jump attack, and a throw when striking a staggered enemy at close range. Knockdowns rotate the body 90 degrees. Knights block frontal strikes; hit them during their attacks or from behind. Boss has a red HUD bar, higher HP, and wider reach.

## Enemies and encounters
Squad-gated camera locks: the stage scrolls until a squad triggers, the camera locks, and the "GO" arrow returns when the squad is cleared. Thugs (tan/green/red variants), rising skeletons, shield knights, beast riders (knock the rider off to mount), pot-carrying thieves, and the boss.

## Magic system
Pots collected from thieves and drops fill the HUD pot row; the pot count sets the spell level (capped per hero). Casting consumes all pots: barbarian fire pillars on every enemy, dwarf lightning bolts, amazon dragon flyby. Higher level = more damage.

## Visual system
81 hand-drawn pixel parts assembled into paper-doll frames per character, rendered into a 320x180 buffer and scaled 3x with smoothing off. Procedural stage backdrops with parallax (sky gradient, mountain range, mid-layer trees/huts/bridge/castle, speckled ground). Palette variants recolor thugs, knights, thieves, and beasts. Original arcade-style HUD: STAGE, MAGIC pots + LV, SCORE, portrait + 10 blue life segments, spare-life heads, CREDIT 1, boss bar.

## Controls and accessibility
Pointer-capture touch pad and Strike/Jump/Magic buttons; portrait stacks game above controls, landscape overlays them. Keyboard: arrows/WASD, J/K/L, P pause. No network calls, accounts, or personal data. Audio is synthesized WebAudio, mutable by pausing.

## Release and verification
GitHub Pages serves `main` root; keep README, this PRD, and code updated in the same round with atomic commits. Verify the live deployed build at 390x844 portrait and 844x390 landscape before reporting. A physical phone check is still pending; do not claim device-tested.

## Decisions, 2026-09-27 (round 2)
- Rebuilt the entire renderer as hand-drawn pixel art (parts + paper-doll frames) after the vector-block pass failed the arcade-fidelity bar.
- Added the genre-defining systems the first pass lacked: depth lanes, squad-gated scrolling, rideable beasts, thieves and pots, leveled magic, knights that block, boss bar, stage intro cards.
- Fidelity is measured screen-by-screen against original arcade reference screenshots used as reference only; no pixels, audio, names, or code were copied.
