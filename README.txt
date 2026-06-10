BobLimt runtime folder

Run BobLimt.exe and accept the admin prompt.
Extract the full folder before running. Do not run the exe from inside the zip preview.

Required files:
- BobLimt.exe
- WinDivert.dll
- WinDivert64.sys
- BobLimt.cfg
- qbtxr54.xaml
- MapleMono-Bold.ttf

BobLimt writes settings to BobLimt.cfg and launch diagnostics to BobLimt.launch.log in this folder.
The release exe is statically linked with the C++ runtime, so no Visual C++ redistributable install should be needed.

Notes:
- Start Destiny 2 before launching BobLimt.
- The main window appears on the taskbar.
- The _ button minimizes BobLimt to the system tray.
- Drag the title area of app windows to move them.
- The overlay only appears while Destiny 2 is the foreground app.
- Settings stores your display name, Bungie ID, overlay color, clear tracker, and region editor options.
- Preferences stores 3074/27k buffering and auto-resync, 30k slow buffering, and Load Manipulation duration/auto manipulation.
- Keybinds support combos like Ctrl+Shift+H.
- Swaps has profile tabs, an Inventory bind, an Open loadouts bind, and typed number boxes. Click a number, type, then press Enter.
- Swaps pixel capture: open Swaps, click Start Editing, press Shift+0, then click loadout slots 1 through 20.
- Future updates are checked on launch through the public binary repo and applied from the full package zip when the version is newer.