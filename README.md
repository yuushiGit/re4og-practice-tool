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

4 save slots that snapshot the entire game state in memory. Save with **F5**, load with **F6** for instant restore with no loading screens. States can only be loaded in the same room where they were saved. Leaving the room or triggering an event invalidates them.

### Backups

Backup and restore your .sav files without leaving the game. Export with a custom filename, browse your backups, rename, delete, or apply them. Useful for preserving progress before experimenting.

### Collision Display

Toggle hitboxes, individual body parts, attack hitboxes, terrain collision geometry, event trigger areas, and room info overlays. Each category has a per-type filter so you can show only the types you need.

### HP & Damage

Show HP values in a side panel with color-coded health bars. Overhead bars appear above enemies in the game world. Floating damage numbers pop up on every hit.

### Speedrun Timer

A large on-screen timer with start/stop/reset controls. Auto-start on room loads or savestate loads. Reset displays the previous time in the OSD before returning to zero.

### Inventory Editor

A visual attache case grid with drag-and-drop, rotation, and collision guides. Add any item from a searchable dropdown sorted by category. Edit ID, quantity, ammo, and orientation. Key items and treasures are listed separately.

### Cheats

Toggle cheats like invincibility, noclip, free camera, and speed override. Includes action buttons for checkpoint management, save game, open merchant, debug trigger, and back to title. All cheats can be bound to hotkeys.

### Area Jump

Warp to any room organized by scenario: Village, Castle, Island, Separate Ways, Assignment Ada, and Mercenaries. The current room is auto-selected when you change areas. Rooms have a search filter for quick lookup.

### Memory Patches

Skip intro logos, door animations, save screen transitions, the quit fade-out, and the Krauser knife-fight QTE. All patches are toggleable from the Patches tab. Changes require a game restart to take effect.

### Hotkeys

Every function can be bound to a keyboard key, combo, or gamepad button. Hover any keybind button for instructions.

| Key | Action |
|-----|--------|
| F5 | Save State |
| F6 | Load State |
| F10 | Toggle Overlay |

All other hotkeys are unbound by default.

### Info Panel

Displays room name, chapter, difficulty, dynamic difficulty, in-game time, money, kill count, and accuracy. Also shows player position and a live RNG graph for analysis.

## Compatibility

- Resident Evil 4 UHD (2014 Steam version)
- Tested on v1.1.0
- Linux/Proton compatible (font fallback included)

## Credits

- [re4_tweaks](https://github.com/nipkownix/re4_tweaks) — Reference for game structures and memory patterns
- [re4-research](https://github.com/emoose/re4-research) — Reverse engineering research
- [Dear ImGui](https://github.com/ocornut/imgui) — UI framework
