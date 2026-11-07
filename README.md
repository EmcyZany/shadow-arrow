# SHADOW ARROW: Hunter of Shadows

A 2D silhouette archery game for mobile and desktop. You are the last Shadow
Archer. Dark shadow enemies have taken over the forest and hide on trees and
rooftops — and some stand on the ground right in front of you, facing you
down. Kill them all and survive 70 levels.

## Play it

- Live: https://shadow-arrow-lovat.vercel.app
- Or open `index.html` in any browser — the whole game is one self-contained
  file (HTML, CSS, JavaScript, Canvas). No build step, no server needed.
- Menu music: the homepage loops `menu-music.mp3` (a 26-second song) — but
  only on the main menu. The moment a level starts, the menu song stops and
  the in-game song (Web Audio) plays alone, and it keeps playing on the Game
  Over screen too. The file is hosted with the live deployment; place a copy
  next to `index.html` to hear it when opening the file directly. Without it
  the game still plays, just with no menu song.

## How to play

- **Touch down and drag** — the bow starts facing right, toward the enemies. Drag in the opposite direction to where you want to shoot (drag left to shoot right, drag down from the top right to shoot up right), and the further you pull, the more power. A dotted line shows the trajectory (Levels 1–3 only — from Level 4, aim by feel). **Release** to shoot. Arrows fly with real gravity.
- The archer and the enemies are pure-black vector shadow humans — the draw hand grips the red nock of the arrow and pulls it back to the cheek, then snaps forward on release. Enemies draw the same way before they fire.
- **Headshot = instant kill** (+100). Body hits hurt: 2 hits to kill (+50).
- Enemies shoot back. Each hit costs 25 HP. 0 HP = game over.
- **Spawn pacing:** new enemies arrive on a level-paced timer — slowly at
  first (one group every 3 seconds on levels 1–2), faster as you advance
  (every 0.42s by level 45), and never faster than every 0.1s from level 51
  on. The first group of a level still arrives quickly so a level never
  starts empty. Enemies already on the field keep shooting at you the whole
  time.
- **Beat all 70 levels** and a victory popup appears with a **Tweet Your
  Victory** button — it opens X with your win pre-filled (🏹 SHADOW ARROW:
  Hunter of Shadows + the link to the deployment you played on), ready for
  you to post. The popup only appears after level 70.
- **Ground enemies:** some enemies stand on the ground line right in front
  of you, on the same level as you and facing you — like a duel — in addition
  to the ones up on rooftops and trees. They shoot at you from ground level
  with the same telegraph and ballistic aim. Bosses stay on their platform.
- **Wind** bends your arrows — watch the WIND meter. **Bosses** appear every
  10 levels. Rainy levels, moving targets, shielded enemies, and headshot
  combos keep the later levels dangerous.
- **Falling pickups (from level 11):** about 1 in 3 levels, a heart ❤️ or a
  shield 🛡️ drifts down — shoot it to collect it. Hearts heal +25 HP,
  shields block the next enemy hit.
- **Pause** with the ⏸️ button in the top bar (the game also pauses itself if
  you switch away). **Mute** with the 🔊 button — the homepage has one too.
- **Landscape mode:** on a PC or desktop the game opens in landscape by
  default — a wide view (up to 960px, 16:9) instead of a portrait column.
  Rotate your phone and the game fills the wide screen — enemies spread out
  across the field instead of bunching up. The top bar compacts to one row
  and every menu compacts to fit the wide box without scrolling (two-column
  menu buttons, two-column weapon/achievement lists, a 14-column level grid).
  Rotate back any time; the level keeps running, nothing resets. Portrait
  phones still get the portrait layout.
- Enemies at the far edge of a wide screen can reach you: their arrows use
  a ballistic arc (extra speed for long shots, so the arrow lands on you
  instead of falling short), and every enemy arrow — including the boss's
  3-arrow burst — points along its flight path toward you.
- Spend coins in the **Shop** on health, arrow speed and blast radius
  upgrades. Unlock **10 weapons** as you level up (or buy them early with
  coins): Swift, Triple, Flame, Five Burst, Bomb Throw, Explosive, Ice,
  Seeking and Shadow Piercer. Seeking (Level 45) and Shadow Piercer
  (Level 70) are earned only — they are never for sale, and once unlocked
  they can be used on any level. Seeking arrows curve toward the nearest
  enemy; Shadow Piercer arrows pass straight through a line of enemies.
  The Bomb is thrown overhand, not shot from a bow.
- **Weapon selection:** pick your weapon on the **WEAPONS** page from the
  main menu — your selected weapon is listed first and marked RECOMMENDED.
  It stays equipped until you are killed (no switching mid-game). When you
  are killed, the Game Over screen lets you **Change Weapon**, then press
  Back and **Retry Level** to play again with the new weapon.
- Progress, coins, weapons, upgrades, mute setting and achievements save
  automatically in the browser (LocalStorage).

## Credits

Made by Samuel — follow the dev on X: https://x.com/Samuelcheq1

## Tech

Single-file HTML5 Canvas game, plus the `menu-music.mp3` song file. Web Audio
API for all in-game sounds (synthesized) plus a quiet music loop. Touch and
mouse controls. On a PC or desktop the game opens in a wide landscape view
by default; portrait phones use a centered portrait layout. Rotate a phone
to landscape and the game fills the wide screen, spreading the enemies out.
No dependencies.
