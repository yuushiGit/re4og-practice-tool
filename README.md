# RE4OG Practice Tool

A practice and analysis mod for Resident Evil 4 UHD on Steam. Drop a single DLL into your game folder and get an in-game overlay with savestates, collision display, a speedrun timer, inventory editing, and more.

![License](https://img.shields.io/badge/license-MIT-blue)

## Installation

1. Download **dinput8.dll** from the [Releases](../../releases) page.
2. Drop it into the same folder as bio4.exe.
3. Start the game — the overlay is ready.

Press **F10** to open the overlay. The game pauses while the overlay is focused — a slide toggle at the top of the window lets you disable this. All settings are saved automatically.

To uninstall, just delete dinput8.dll. The game returns to vanilla.

## Features

### Savestates

4 save slots that snapshot the entire game state in memory. Save with **F5**, load with **F6** — instant restore, no loading screens. States can only be loaded in the same room where they were saved; leaving the room or reloading invalidates them. Saving is blocked during cutscenes and events.

### Backups

Backup and restore your .sav files without leaving the game. Export with a custom filename (timestamp is prefilled), browse your backups, rename, delete, or apply them to restore your save.

### Collision Display

See what the game actually sees. Toggle body outlines, per-part hitboxes, attack ranges for both the player and enemies, event trigger zones, and terrain collision geometry. Capsules are filled with semi-transparent color so overlapping shapes are easy to read.

### HP & Damage

Show HP values in a side panel, overhead bars above enemies, and floating damage numbers on hit.

### Speedrun Timer

A large on-screen timer with start/stop/reset controls. It can auto-start on room loads (including checkpoint retries) or savestate loads. Reset stops the timer and returns it to zero.

### Inventory Editor

A visual grid that mirrors your attache case in real time. Drag items to reposition them, right-click to rotate, click to edit ID, quantity, ammo, or orientation. Key items and treasures are listed separately with edit support. You can also add any item in the game from a dropdown.

The grid automatically adjusts to your current case size (S / M / L / XL).

### Cheats

Invincibility, infinite ammo, weak enemies, noclip, free camera, RNG freeze, and a game speed slider (0.1x to 5.0x). Free camera detaches the view from the player and lets you fly around with WASD, mouse look, Space/Ctrl for vertical movement, and Shift to boost. Quick-action buttons let you save or retry a checkpoint, force a game save, or return to the title screen. Area jump lets you warp to any room organized by stage (Village, Castle, Island, Mercenaries, Separate Ways).

### Memory Patches

Skip intro logos, door animations, save screen transitions, and the quit fade-out. The Krauser knife-fight QTE can also be skipped. Changes require a game restart to take effect.

### Hotkeys

Every major function can be bound to a key. Defaults:

| Key | Action |
|-----|--------|
| F5 | Save State |
| F6 | Load State |
| F10 | Toggle Overlay |

All other hotkeys are unbound by default and can be configured in the Hotkeys tab.

### Info Panel

Displays room name, chapter, difficulty, dynamic difficulty, in-game time, money, kill count, accuracy, player position, and a live RNG graph.

## Compatibility

- Resident Evil 4 UHD (2014 Steam version)
- Tested on v1.1.0

## Credits

This project was made possible by the work of the RE4 modding community.

- [re4_tweaks](https://github.com/nipkownix/re4_tweaks) — Reference for game structures and memory patterns
- [re4-research](https://github.com/emoose/re4-research) — IDA database and reverse engineering research
- [Dear ImGui](https://github.com/ocornut/imgui) — UI framework
