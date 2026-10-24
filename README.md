# NTE-Guitar

**Neverness to Everness Guitar Auto Player**

[한국어 설명](README_KR.md) · [Download Windows v1.4.4](https://github.com/kgp0907/NTE-Guitar-Macro/releases/tag/v1.4.4) · [Song list](docs/SONGS.md)

A portable Windows player for the in-game guitar. Import a MIDI file, choose the musical parts, preview the arrangement, and play through customizable hotkeys.

![Main library and playback controls](screenshots/main.jpg)

## Downloads

| User | Download |
| --- | --- |
| New installation | [v1.4.4 Windows ZIP](https://github.com/kgp0907/NTE-Guitar-Macro/releases/download/v1.4.4/NTE-Guitar-v1.4.4-Windows.zip) — includes the existing 29 default arrangements |
| Existing installation | [v1.4.4 Update ZIP](https://github.com/kgp0907/NTE-Guitar-Macro/releases/download/v1.4.4/NTE-Guitar-v1.4.4-Update-Windows.zip) — preserves your songs, MIDI files and settings |
| Previous version | [v1.0 Windows ZIP](https://github.com/kgp0907/NTE-Guitar-Macro/releases/download/v1.0/NTE-Guitar-v1.0-Windows.zip) · [v1.0 release](https://github.com/kgp0907/NTE-Guitar-Macro/releases/tag/v1.0) |

For updates, fully exit the player, back up the existing folder, and merge the update ZIP's `NTE-Guitar` contents into that folder. Replace the EXE and `_internal` together. Keep `songs`, `sources`, `settings.json` and `ui-state.json`; do not delete the installation folder. Use the full ZIP for a fresh installation.

[Changes since v1.0](docs/CHANGES-v1.4.4-KR.md) · [Shared songs guide](docs/SHARED-SONGS-KR.md) · [Verification](docs/VALIDATION-v1.4.4-KR.md)

## 1.4.4 fix

Fixed missing initial shortcut settings after importing a first song into an empty update-only folder and restarting. See the [fix and existing affected-folder guidance](docs/VALIDATION-v1.4.4-KR.md).

## Features

- Searchable library with separate artist, title, version, recommended tone, and hotkey columns.
- MIDI import and per-track/channel roles: lead melody, supporting melody, chords/rhythm, bass, or exclude.
- Original-part and arranged PC MIDI previews, arrangement presets, chord limits, and octave fitting.
- Click anywhere on the playback slider to seek, then resume from the selected position.
- Sustained key presses and rapid-repeat timing correction, with a fixed F8 stop key.
- Compact HUD with separate Play/Resume, Pause and Stop buttons. Button widths stay fixed when state labels change.
- Favorites, song editing, deletion/restoration, and four interface languages.
- Approved shared songs: online playback, plus offline `.nteplay` import for songs explicitly permitted for file download.
- Right-click a song → **Change shortcut**: see conflicts immediately and pick an available key.

## Quick start

1. Download **NTE-Guitar-v1.4.4-Windows.zip** from [Releases](https://github.com/kgp0907/NTE-Guitar-Macro/releases).
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

## Shared songs and mini player

Open **Shared songs**, choose a song marked as allowing file import, and add it to your library. Assign a hotkey from its context menu to play offline. The `.nteplay` file contains the saved final performance, not the original MIDI or editable part sources. Online-only songs cannot be added as offline files.

Pause keeps the current position; Play/Resume continues from there. **Numpad .** toggles pause/resume by default. **F8** fully stops local songs and returns to the beginning. Stopping an online-only session clears its session data; load it again from Shared songs.

## Screenshots

### Arrangement editor

![Part selection and arrangement preview](screenshots/arrangement.jpg)

### Mini HUD

![Mini HUD](screenshots/hud.jpg)

### Song shortcut editor

![Available keys and shortcut validation](screenshots/shortcuts.jpg)

Screenshots are from the initial release, captured with game input and global hotkeys disabled. The current mini HUD has three separate transport buttons with stable widths.

## Files and source availability

```text
README.md / README_KR.md   Project introduction
screenshots/              Application screenshots
docs/                     Song list, credits and release notes
GitHub Releases           NTE-Guitar-v1.4.4-Windows.zip
```

The Windows release includes the latest cumulative Fix5 executable. Application source code and repair scripts are kept private and are not included in this public repository or its downloads.

Windows 10/11 x64 is required. Playback depends on game focus, system load, and how the game accepts simulated keyboard input. This is an unofficial utility and does not patch game files or game memory. The build is unsigned; unknown-publisher warnings are not a malware-scan result. Verify the release source and SHA-256 checksum before use.

Bundled dependency licenses are in `licenses/` in the Windows ZIP. Song/transcription credits and available source links are retained in the score metadata and [credits list](docs/CREDITS.md). No blanket license for third-party musical material is granted by this repository.
