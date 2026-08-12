# Guild Rancher — playtest build

Compiled WebGL output only. Source lives in the private `Guild-Rancher` repo.

**A LOOK-AT-IT LINK, NOT A PERF MEASUREMENT.** This runs in a browser, which is
the sandbox the Unity fork exists to get out of. Frame times here say nothing
about what the engine does natively — that answer needs the APK.

## What this build holds (2026-08-12)

- **Combat.** The web build's own numbers, transcribed: d20 + stat mod + prof
  vs 10+dex AC, hp 20+CON×2, crits double the dice, a hit is never free. One
  resolver answers the player's swing, the AI's decision and the HUD readout.
  Foes close to whip reach and fight back; the HUD shows your hp and the last
  blow's arithmetic.
- **Three lenses on V.** Over the shoulder → first person (the delve's own eye
  height; you are the one billboard not drawn) → top-down. Same world, same
  assets, same sizes in all three.
- **Everyone is generated.** Twelve armed fighter looks and twenty-four
  townsfolk in the stands, out of the web build's own character generator —
  same tables, same rng, same person per seed. No more six tinted clones.

## Controls

| desktop | |
|---|---|
| WASD / arrows | move (screen-relative) |
| Space | swing |
| right-drag / wheel | look / zoom |
| V | lens · C crowd · F field · R re-roll |
| Tab | batched ⇄ GameObject render path |
| [ / ] | fewer / more fighters |

Touch: left half drags to walk, right half to look, pinch zooms, buttons down
the right edge mirror the toggles.
