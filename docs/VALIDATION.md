# Release verification — v1.0

- 29 arrangements, 116 song/rate cases and 237,780 simulated note attacks checked.
- Score onsets and chord attacks retained by the playback timing layer.
- Seek, held notes, pause/resume, emergency stop and preview-message cleanup passed.
- Live shortcut validation, free-key enumeration, full/quick dialog save/cancel, and right-click row selection passed.
- Repaired EXE rebuilt from the published repair modules is byte-identical to the packaged EXE.
- The actual main, arrangement, HUD and shortcut widgets were captured with input/global hooks disabled.
- A free-key button was clicked and its immediate available-key feedback was observed; no settings were saved in that session.
- Original MIDI references included in the ZIP resolve inside its sources directory.
- Existing active song files were not changed while assigning keys; old executables and settings are backed up outside the program directory.

Checks simulate game input and MIDI output. Actual game acceptance and audible output were not verified in this preparation. The build is unsigned; no completed malware-scan result is claimed.
