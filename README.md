# EQ UI Workbench

A browser-based editor for EverQuest (Live / Legends) UI skins and window layouts. Everything runs locally in your browser — no install, no server, and your files never leave your computer.

**Open it:** https://eqhafa.github.io/eq-ui-workbench/

## What it does

**Screen layout** — loads your `UI_<character>_<server>.ini` (and `eqclient.ini` for resolution and UI scale) and draws every window where the game puts it.
- Drag and resize windows with the skin's real size rules (min/max sizes, grid-snapping windows like hotbars and spell bars).
- Snap to screen edges, other windows, or a grid — using either the defined edge or the visible edge of the skin art.
- Lock, group and attach windows; box select; align, distribute and match sizes.
- Handles display types (e.g. `PlayerWindow_5`), KeepOnScreenOffset and loadout files (`_LO1`, `_LO2`, …).

**Window designer** — opens the SIDL XML for any window in your skin (`uifiles/<skin>/EQUI_*.xml`).
- See the window rendered with the skin's textures (TGA and DDS).
- Select pieces, edit properties, duplicate and delete controls.
- Grid helpers and "fit to contents" for tile-layout windows such as the spell bar.

## Saving

The Workbench never writes to your game folder. Saving downloads a `.zip` containing the changed files **plus a `_backup_<date>` folder with your untouched originals**. Copy the files into your EverQuest folder yourself, then `/loadskin <skin>` in game.

## Getting started

1. Open the page in Chrome, Edge or Firefox.
2. **Screen layout:** click *Open layout .ini* and pick your `UI_*.ini` (and `eqclient.ini`) from your EverQuest folder.
3. **Skin art and the Window designer:** click *Open uifiles folder* and pick your `uifiles` folder, then choose your skin from the *Skin* list.
4. Edit, then *Save* and *Download .zip*.

## Notes

- Not affiliated with or endorsed by Daybreak Game Company. EverQuest is a registered trademark of Daybreak Game Company LLC. No game files are included; the tool only reads files you choose.
- Layout and skin data stay in your browser. A few editor preferences (locks, groups, calibrations) are kept in your browser's local storage.

## License

CC0 1.0 Universal (public domain dedication). See [LICENSE](LICENSE).
