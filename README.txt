BobLimt runtime folder

Run "Launch BobLimt.vbs" to start BobLimt elevated, or run BobLimt.exe directly and accept the admin prompt.
Extract the full folder before running. Do not run the exe from inside the zip preview.

Required files:
- BobLimt.exe
- WinDivert.dll
- WinDivert64.sys
- BobLimt.cfg

BobLimt writes settings to BobLimt.cfg and launch diagnostics to BobLimt.launch.log in this folder.
The release exe is statically linked with the C++ runtime, so no Visual C++ redistributable install should be needed.

Notes:
- Start Destiny 2 before launching BobLimt.
- The main window appears on the taskbar.
- The _ button minimizes BobLimt to the system tray.
- Drag the title area of app windows to move them.
- The overlay only appears while Destiny 2 is the foreground app.
- Preferences stores 3074/27k buffering and auto-resync, 30k slow buffering, and Load Manipulation duration/auto manipulation.
- Preferences has Allow background binds. By default binds only trigger while Destiny 2 is foreground.
- Settings toggles overlay arrows and active-second counters. Set confined active region opens a drag-and-save editor for the timer and module blocks.
- Keybinds support combos like Ctrl+5. Click a bind, hold the modifier, press the trigger key, or press Esc to clear.
- Swaps has an Inventory bind box and typed number boxes. Click a number, type, then press Enter.
- Swaps ticks selected-port UL, optionally 3074 DL, performs the swaps, then unticks after Untick Delay.
- Swaps pixel capture: open Swaps, click Start Editing, focus Destiny 2, press Shift+0, then click loadout slots 1 through 20.
