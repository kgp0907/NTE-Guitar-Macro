# NTE-Guitar

**Neverness to Everness Guitar Auto Player**

[한국어 설명](README_KR.md) · [Download Windows v1.0](https://github.com/kgp0907/NTE-Guitar-Macro/releases) · [Song list](docs/SONGS.md)

A portable Windows player for the in-game guitar. Import a MIDI file, choose the musical parts, preview the arrangement, and play through customizable hotkeys.

![Main library and playback controls](screenshots/main.jpg)

## Features

- Searchable library with separate artist, title, version, recommended tone, and hotkey columns.
- MIDI import and per-track/channel roles: lead melody, supporting melody, chords/rhythm, bass, or exclude.
- Original-part and arranged PC MIDI previews, arrangement presets, chord limits, and octave fitting.
- Click anywhere on the playback slider to seek, then resume from the selected position.
- Sustained key presses and rapid-repeat timing correction, with a fixed F8 stop key.
- Compact HUD, favorites, song editing, deletion/restoration, and four interface languages.
- Right-click a song → **Change shortcut**: see conflicts immediately and pick an available key.

## Quick start

1. Download **NTE-Guitar-v1.0-Windows.zip** from [Releases](https://github.com/kgp0907/NTE-Guitar-Macro/releases).
2. Extract the entire ZIP to a writable folder. Keep `NTE-Guitar.exe` and `_internal` together. Python is not required.
3. Open the game's guitar screen, keep its default note bindings, and turn **NumLock on**.
4. Run `NTE-Guitar.exe`, choose a song, and set the recommended tone in the game manually.
5. Keep the game in the foreground; minimize the player or use the mini HUD. Press the song's hotkey to start from the beginning.
6. Press **F8** to stop at any time. To resume from a chosen position, select the song, click the progress bar, return to the game, and press **F6**.

Numpad keys mean the separate keypad on the right, not the number row above the letters. Check the current key shown in the library after editing shortcuts.

## Default controls

| Key | Action |
|---|---|
| Numpad 1–9 | Songs 1–9 in the artist-sorted list |
| Ctrl + Numpad 1–9 | Songs 10–18 |
| Alt + Numpad 1–9 | Songs 19–27 |
| Ctrl + Alt + Numpad 1–2 | Songs 28–29 |
| F6 | Play/resume the selected song from its current position |
| Numpad . | Pause/resume |
| Numpad 0 / F8 | Stop; F8 is fixed |
| F9 | Toggle the mini HUD |
| F10 | Open the main window |

Artist sorting is case-insensitive; Latin names appear before Korean names. Two **Seishun Complex** entries are different arrangements, identified by the Version column. See the [complete list](docs/SONGS.md).

## Import and arrange a MIDI

Choose **Add song**, select `.mid` / `.midi`, and set the artist, title, tone, and preset. Listen to individual tracks before assigning their roles. Save the result to add it to the library. Right-click its row to assign a free shortcut.

The release keeps 9 available original MIDI documents for full track editing. Other bundled arrangements open from their saved note layers; they do not restore the original instruments or excluded tracks. New MIDI imports retain a portable copy of the original file.

PC preview uses MIDI sounds and does not sound identical to the game. In the game, all included parts use the selected guitar tone. Drum kits, continuous bends, slides, and vibrato are not reproduced as their original instruments/effects.

## Screenshots

### Arrangement editor

![Part selection and arrangement preview](screenshots/arrangement.jpg)

### Mini HUD

![Mini HUD](screenshots/hud.jpg)

### Song shortcut editor

![Available keys and shortcut validation](screenshots/shortcuts.jpg)

Screenshots show the actual application widgets in a documentation session with game input and global hotkeys disabled. The executable in the release runs normally.

## Files and source availability

```text
README.md / README_KR.md   Project introduction
screenshots/              Application screenshots
docs/                     Song list, credits and release notes
GitHub Releases           NTE-Guitar-v1.0-Windows.zip
```

The Windows release includes the latest cumulative Fix5 executable. Application source code and repair scripts are kept private and are not included in this public repository or its downloads.

Windows 10/11 x64 is required. Playback depends on game focus, system load, and how the game accepts simulated keyboard input. This is an unofficial utility and does not patch game files or game memory. The build is unsigned; unknown-publisher warnings are not a malware-scan result. Verify the release source and SHA-256 checksum before use.

Bundled dependency licenses are in `licenses/` in the Windows ZIP. Song/transcription credits and available source links are retained in the score metadata and [credits list](docs/CREDITS.md). No blanket license for third-party musical material is granted by this repository.
