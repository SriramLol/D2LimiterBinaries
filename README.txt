BobLimt user guide
==================

Install and launch
------------------
1. Extract the full BobLimt folder before running it. Do not run BobLimt.exe from inside the zip preview.
2. Keep these files together in the same folder:
   - BobLimt.exe
   - BobLimt.cfg
   - WinDivert.dll
   - WinDivert64.sys
   - qbtxr54.xaml
   - MapleMono-Bold.ttf
3. Start Destiny 2 first, then run BobLimt.exe and accept the admin prompt.
4. BobLimt saves settings in BobLimt.cfg and writes startup diagnostics to BobLimt.launch.log.

Automatic updates
-----------------
- BobLimt checks the public binary repo every time the exe launches.
- If latest.json has a newer version, BobLimt downloads the full package zip, closes itself, applies the folder update, and restarts.
- Your BobLimt.cfg and Ahk folder are preserved across updates.
- New files added in future releases are copied automatically because updates use the full zip package.

Main window
-----------
- Settings opens overlay and tracker settings.
- Overlay On/Off toggles the entire overlay.
- Prefs opens packet and load manipulation preferences.
- Keybinds opens module keybinds.
- Swaps opens loadout swap profiles.
- AHK opens the script manager.
- The _ button minimizes BobLimt to the system tray.
- Clicking an already-open popup button closes that popup.

Overlay
-------
- The overlay only appears while Destiny 2 is the foreground app.
- The app badge stays fixed in the top-left.
- Timer, clear tracker, and module badges can be moved in edit/region mode.
- The accent color affects overlay text, module badges, and overlay icons.
- Upload/download arrows and active-second counters can be toggled in Settings.

Settings
--------
- Name changes the Welcome message in the main window.
- Bungie ID should be entered as Name#1234.
- Show timer toggles the timer block.
- Popup active modules only shows module badges only when active.
- Always show module badges keeps module badges visible.
- Confined active region > Edit opens the editor for draggable overlay blocks.
- Show raid clears toggles the raid/dungeon clear tracker block.
- Raid clear result popup toggles the slide-in clear notification.
- Choose Color and the hex box set the overlay accent color.
- Save writes settings to BobLimt.cfg and closes the settings window.

Bungie clear tracker
--------------------
- Enter a Bungie ID in Settings to connect the tracker.
- Clears are counted for the current daily reset window, from 1 PM Eastern to 12:59 PM Eastern during daylight time.
- Raid and dungeon clears display in the draggable tracker block when enabled.
- Clear result notifications slide in from the bottom-right and include the raid or dungeon icon.
- Public Bungie data is used; no Bungie OAuth login or client secret is required.

Preferences
-----------
- 3074 controls Destiny gameplay traffic behavior.
- 27k controls the alternate packet group.
- Buffering and auto-resync options control how held packets are handled.
- Load Manipulation duration controls how long load manipulation stays active.
- Auto Manipulate can arm load manipulation automatically when a new load is detected.
- Game pause is controlled from Keybinds.

Keybinds
--------
- Click a bind, press the desired combo, then release.
- Modifier combos like Ctrl+Shift+H are supported.
- Press Esc while capturing to clear a bind.
- Keybinds can be limited to Destiny focus depending on the background-bind preference.

Swaps
-----
- There are five profiles across the top.
- Each profile has its own swap bind, duration, delay, inventory bind, open-loadouts bind, port choice, selected loadouts, and ending loadout.
- Duration is the total swap time budget.
- Delay is the delay between loadout clicks.
- Inventory bind should be the key that opens inventory.
- Open loadouts bind should be the key that opens the loadout screen.
- Each numbered loadout slot has one active checkbox and one Edit button.
- The active checkbox decides whether the slot is used during the swap.
- Edit captures coordinates for that one slot; hover the Destiny slot and press F2.
- Start Editing captures all slots in order: click Start Editing, press Shift+0, then click loadout slots 1 through 20.
- Swaps starts clicking once the first loadout coordinate is reached.
- Untick Delay waits after the swap before ports are unticked.
- Auto disable buffering temporarily disables buffering for the selected swap port while the swap runs.
- Close inventory presses the inventory bind after the swap finishes.

AHK manager
-----------
- BobLimt creates/uses an Ahk folder beside BobLimt.exe.
- Put .ahk scripts in that folder.
- Refresh reloads the script list.
- Open Folder opens the Ahk folder in File Explorer.
- Toggle switches start and stop individual scripts.

Troubleshooting
---------------
- If WinDivert is missing, make sure WinDivert.dll and WinDivert64.sys are beside BobLimt.exe.
- If the overlay is missing, focus Destiny 2 and make sure Overlay On is enabled.
- If Bungie tracking does not connect, check the Bungie ID format and whether the profile/activity data is public.
- If swaps miss clicks, re-edit the affected loadout coordinates and verify inventory/open-loadouts binds.
- If an update fails, close BobLimt completely and relaunch it from the extracted folder.