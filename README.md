# Garfield's Lasagna Hunt – play in a browser

A personal, non-commercial SNES fan game made for Andy. All the pixel art, music and code are original. Garfield has to track down the biggest lasagna in town across six levels.
It runs in the browser with EmulatorJS (snes9x core) and is set up for an iPad in Safari, with on-screen touch buttons.

**Play:** https://xao214.github.io/garfield-lasagna-hunt/

## Running it
Open the link above in Safari (or any modern browser). On an iPad, tap **Share → Add to Home Screen** to get a full-screen app icon.

To run your own copy, serve this folder over http, e.g. `python3 -m http.server 8000`, then open http://localhost:8000/. Opening `index.html` straight from disk (file://) won't work. Everything it needs is in the folder, so no internet connection is required.

On an iPad: hold it in landscape, tap **Tap to start**, and use the on-screen buttons. **?** (top left) shows the controls and pauses; ☰ (top right) opens the emulator bar (pause, restart, save/load state, mute/volume, full screen). Share → Add to Home Screen gives a full-screen icon.

## Controls
| Button | Action |
|---|---|
| D-pad left/right | Walk (you walk up stairs automatically) |
| B or A | Jump (hold to jump higher) |
| Y or X | Pounce, a dash that stuns enemies |
| Down + jump | Drop through a one-way platform (shelves, tables, branches) |
| Start | Pause / confirm; on Game Over, continue |
| Select (title) | Enter a password |

Keyboard: arrows, X = B, Z = A, S = Y, A = X, Enter = Start, V = Select. Bluetooth game controllers also work.

Stomping on an enemy or pouncing into it stuns it. Touching an awake enemy costs a heart.

## Items
* **Cookie:** 10 points; every 50 cookies gives an extra life.
* **Pizza:** 500 points and a heart back. **Heart:** 100 points and a heart back.
* **Coffee:** a few seconds of speed boost.
* **Key:** opens a locked door or gate.
* **Pooky:** give him to Odie and Odie moves out of the way.
* **Beds and cushions:** checkpoints; you respawn at the last one you napped on.
* **Lasagna:** in the kitchen finale, after you beat Brutus.

## Levels and passwords
1. Jon's House
2. Back Garden – `NAPS`
3. The Street – `MAIL`
4. The Park – `POOK`
5. Pet Shop / Vet – `LIZY`
6. Kitchen finale, boss fight with Brutus the bulldog – `YUMS`

**Brutus** winds up and charges, then crashes into a counter and goes dizzy. Pounce or stomp him while he's dizzy (3 hits). You can hide from his charge on the worktops.

## Notes
* Save states are kept in that browser on that device.
* On iPad, sound starts after the first tap.

## Files
* `index.html` – page and EmulatorJS settings (touch layout, trimmed menu, tap to start).
* `rom/garfield-snes.sfc` – the game (512 KB LoROM).
* `data/` – EmulatorJS 4.2.3 (loader, emulator, snes9x core). EmulatorJS is GPL-3.0; the snes9x core is for non-commercial use.

Garfield and related characters belong to their owners. This is an unofficial fan game for personal use only.
