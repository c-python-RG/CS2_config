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

1. Copy the text of your updated configuration script.
2. Save it as a new file named `UltimateCs2.cfg`.
3. Move this file into your Counter-Strike 2 `cfg` directory.
4. Launch Counter-Strike 2, open your developer console (`~`), and type `exec UltimateCs2` to load the environment.

## Controls & Keybinds

**Practice Environment Controls**
* **`B`**: Toggle Noclip (Flying)[cite: 1]
* **`N`**: Rethrow your last practice grenade[cite: 1]
* **`I`**: Kick all bots and clear the map[cite: 1]
* **`P`**: Instantly restart the practice round[cite: 1]
* **`Y`**: Print the control menu into the chat[cite: 1]

**Interactive Spawn Navigation**
* **`UPARROW`**: Cycle through active maps (Mirage, Ancient, Inferno, Nuke, Anubis, Cache)[cite: 1]
* **`DOWNARROW`**: Toggle between CT and T sides[cite: 1]
* **`RIGHTARROW`**: Teleport to the next spawn lineup[cite: 1]
* **`LEFTARROW`**: Teleport to the previous spawn lineup[cite: 1]

## ⚠️ Crash Prevention Guide: The `O` Key / Bot Placement Feature

The Source 2 engine will instantly crash if you attempt to place a bot's 3D model inside your own player model or inside the map geometry. To prevent this, the `O` key uses a two-step safety toggle[cite: 1].

* **Step 1 (Add)**: Press `O` once. The script will generate a frozen bot in the background and print a warning[cite: 1].
* **Step 2 (Move)**: Physically step backward or move your crosshair away from your feet. Never aim directly straight down.
* **Step 3 (Place)**: Press `O` a second time while aiming at a valid, solid floor[cite: 1]. The bot will teleport to where you are aiming.

> **Important:** Never press the `O` key while flying outside the map in Noclip mode. Always drop to a physical floor first!