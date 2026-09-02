// ╔══════════════════════════════════════════════════╗
// ║                                                                 ║
// ║                                 _   _                           ║
// ║        ___          _ __  _   _| |_| |__   ___  _ __            ║
// ║       / __|        | '_ \| | | | __| '_ \ / _ \| '_ \           ║
// ║      | (__  _____  | |_) | |_| | |_| | | | (_) | | | |          ║
// ║       \___||_____| | .__/ \__, |\__|_| |_|\___/|_| |_|          ║
// ║                    |_|    |___/                                 ║
// ║                                                                 ║
// ╠══════════════════════════════════════════════════╣
// ║  Author:      R_G (c_python)                                    ║
// ║  Project:     Ultimate CS2 Practice Environment                 ║
// ║  Build Date:  September 2026                                    ║
// ╚══════════════════════════════════════════════════╝

# CS2 Ultimate Practice & Spawn Selection Config

This configuration file turns a standard Counter-Strike 2 offline server into a fully featured practice environment. It includes a custom interactive spawn-teleportation tree and a built-in safety sequence for placing reference bots.

## Installation Instructions

1. Download the `UltimateCs2.cfg` & `UltimateCs2_Readme.txt`.
2. Move this file into your Counter-Strike 2 `cfg` directory.
3. Launch Counter-Strike 2, open your developer console (`~`), and type `exec UltimateCs2` to load the environment.

## Controls & Keybinds

**Practice Environment Controls**
* **`B`**: Toggle Noclip (Flying)
* **`N`**: Rethrow your last practice grenade
* **`O`**: Bot Placement Feature (Read Caution below)
* **`I`**: Kick all bots and clear the map
* **`P`**: Instantly restart the practice round
* **`Y`**: Help

**Interactive Spawn Navigation**
* **`UPARROW`**: Cycle through active maps (Mirage, Ancient, Inferno, Nuke, Anubis, Cache)
* **`DOWNARROW`**: Toggle between CT and T sides
* **`RIGHTARROW`**: Teleport to the next spawn lineup
* **`LEFTARROW`**: Teleport to the previous spawn lineup

## ⚠️ Crash Prevention Guide: The `O` Key / Bot Placement Feature

The Source 2 engine will instantly crash if you attempt to place a bot's 3D model inside your own player model or inside the map geometry. To prevent this, the `O` key uses a two-step safety toggle.

* **Step 1 (Add)**: Press `O` once. The script will generate a frozen bot in the background and print a warning.
* **Step 2 (Move)**: Physically step backward or move your crosshair away from your feet. Never aim directly straight down.
* **Step 3 (Place)**: Press `O` a second time while aiming at a valid, solid floor. The bot will teleport to where you are aiming.

> **Important:** Never press the `O` key while flying outside the map in Noclip mode. Always drop to a physical floor first!
