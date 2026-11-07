# SHADOW ARROW: Hunter of Shadows

A 2D silhouette archery game for mobile and desktop. You are the last Shadow
Archer. Dark shadow enemies have taken over the forest and hide on trees and
rooftops. Kill them all and survive 70 levels.

## Play it

- Live: https://shadow-arrow-lovat.vercel.app
- Or open `index.html` in any browser — the whole game is one self-contained
  file (HTML, CSS, JavaScript, Canvas). No build step, no server needed.
- Menu music: the homepage loops `menu-music.mp3` (a 26-second song). The
  file is hosted with the live deployment; place a copy next to `index.html`
  to hear it when opening the file directly. Without it the game still plays,
  just with no menu song.

## How to play

- **Touch down and drag** — the bow starts facing right, toward the enemies. Drag in the opposite direction to where you want to shoot (drag left to shoot right, drag down from the top right to shoot up right), and the further you pull, the more power. A dotted line shows the trajectory (Levels 1–3 only — from Level 4, aim by feel). **Release** to shoot. Arrows fly with real gravity.
- The archer and the enemies are pure-black vector shadow humans — the draw hand grips the red nock of the arrow and pulls it back to the cheek, then snaps forward on release. Enemies draw the same way before they fire.
- **Headshot = instant kill** (+100). Body hits hurt: 2 hits to kill (+50).
- Enemies shoot back. Each hit costs 25 HP. 0 HP = game over.
- **Wind** bends your arrows — watch the WIND meter. **Bosses** appear every
  10 levels. Rainy levels, moving targets, shielded enemies, and headshot
  combos keep the later levels dangerous.
- **Falling pickups (from level 11):** about 1 in 3 levels, a heart ❤️ or a
  shield 🛡️ drifts down — shoot it to collect it. Hearts heal +25 HP,
  shields block the next enemy hit.
- **Pause** with the ⏸️ button in the top bar (the game also pauses itself if
  you switch away). **Mute** with the 🔊 button — the homepage has one too.
- Spend coins in the **Shop** on health, arrow speed and blast radius
  upgrades. Unlock **10 weapons** as you level up (or buy them early with
  coins): Swift, Triple, Flame, Five Burst, Bomb Throw, Explosive, Ice,
  Seeking and Shadow Piercer. Seeking (Level 45) and Shadow Piercer
  (Level 70) are earned only — they are never for sale, and once unlocked
  they can be used on any level. Seeking arrows curve toward the nearest
  enemy; Shadow Piercer arrows pass straight through a line of enemies.
  The Bomb is thrown overhand, not shot from a bow.
- Progress, coins, weapons, upgrades, mute setting and achievements save
  automatically in the browser (LocalStorage).

## Credits

Made by Samuel — follow the dev on X: https://x.com/Samuelcheq1

## Tech

Single-file HTML5 Canvas game, plus the `menu-music.mp3` song file. Web Audio
API for all in-game sounds (synthesized) plus a quiet music loop. Touch and
mouse controls. On desktop the game sits in a centered phone-sized column.
No dependencies.
