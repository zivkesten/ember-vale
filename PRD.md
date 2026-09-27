# Ember Vale PRD and handoff

## Goal
A compact original browser beat-'em-up with a striking fantasy arcade appearance and responsive phone controls. Inspired by broad side-scrolling arcade conventions, not a remake or redistribution of Golden Axe.

## Player path
Choose a hero archetype, begin, move through four enemy waves, clear the beacon gate. Three lives and 100 health per life; strike in a three-step combo, jump, cast area magic from finite potion charges. Defeated enemies can drop food or potion bottles. Pause and restart are available.

## Visual system
Canvas pixel blocks, angular silhouettes, rust/amber fantasy palette, layered mountains, old road, trees, stone posts and beacon. Barbarian, dwarf, amazon, skeleton, raider and armored warden are original geometric artwork. The three hero choices share mechanics. No third-party assets, fonts, scripts or sounds.

## Controls and accessibility
Arrow/WASD, J strike, K jump, L magic, P pause. On-screen directional and action buttons use pointer capture for touch. Native button labels describe actions. The canvas is 960 × 540 internally, scaled with pixelated rendering. Portrait stacks stage above touch controls; landscape overlays them. No network request or personal data.

## Release and verification
GitHub Pages serves root of `main`; keep README, this PRD and code in the same change round. Check live portrait at 390 × 844 and landscape at 844 × 390, then a real Android browser before claiming device validation. Rollback by reverting the relevant atomic commit.

## Decisions, 2026-09-27
- Keep Ember Vale name and a typographic title treatment rather than copy a SEGA mark.
- Use deterministic hand-drawn Canvas primitives rather than unlicensed sprites or the educational-only lrusso demo.
- Add cosmetic archetype selection and wave-specific enemy mixtures while retaining established combat controls.
