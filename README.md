# Guild Rancher — playtest build

Compiled WebGL output only. Source lives in the private `Guild-Rancher` repo.

**A LOOK-AT-IT LINK, NOT A PERF MEASUREMENT.** This runs in a browser, which is
the sandbox the Unity fork exists to get out of. Frame times here say nothing
about what the engine does natively — that answer needs the APK.

## The page

The loading screen ends in a button rather than dissolving on its own: the
Fullscreen API only answers a user gesture, so the tap that starts the game is
the tap that spends it. "stay in the page" is beside it for anyone who would
rather not, and the corner mark puts it full screen again later.

Every payload URL carries the build's own stamp (`?v=`), written in by the build
— a redeploy that kept the same four file names was a redeploy a returning phone
could miss.

## What this build holds (2026-08-14)

- **The estate, walked.** The guild is a place: the grounds are a chart you walk
  with every room's interior stamped into the same plane, so a doorway is a gap
  you step through and the roof lifts off the room you are standing in. No
  press, no loading screen, no warp.
- **Rooms with work in them.** The Great Hall's roster, the Grounds, the
  Athanor's board, the Academy's week, the Forge, the Kitchen and the
  Apothecary — reached from inside the building they belong to.
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
