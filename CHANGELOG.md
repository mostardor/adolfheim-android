# Changelog

Versions of the Android port. Dates are YYYY-MM-DD.

## 0.3.4 — 2026-11-27

A smaller app, a new look for the online screen, and a fix for levels that lost their visual effects. Install the new APK over the old one.

### Added
- **What's new** screen after every update (short and color-coded) and a **new version notice** with a download shortcut
- **Online invitation** when the game opens, with the number of players online
- **Drag the screen** in the campaign menu to switch world and area
- **Redesigned online screen:** fewer words, colored buttons, colored rooms and players; *All regions* is on by default
- **Options > Graphics:** *Hide Level Names* and *Hide Hit Judgments* (the *Perfect*, *Late Perfect*... texts)

### Changed
- **About 188 MB smaller** (435.7 MiB APK): ASTC textures; the level editor's Japanese and Chinese fonts were removed
- The pause menu's *Support* button opens the port's Discord

### Fixed
- **Missing visuals and black backgrounds** in levels that use blend effects (Screen, Overlay, Linear Dodge, Difference...),
  like **AR-X Libertas after the drop**: the blend shader only supported three modes and now supports all of them
- Short taps in the campaign menu count when the finger touches the screen (they counted when it was lifted)
- *Back* closes the what's-new window, the online invitation and the update notice instead of opening the pause menu behind them

## 0.3.3 — 2026-11-21

The online rooms are now the same as the PC mod 0.2.10. Install the new APK over the old one.

### Added
- **Up to 8 players per room** (it was 4); the player list and the results window adapt
- **Players online** in the lobby: *Players online · Rooms with players · Active today*
- **Sound when someone joins your room** (not during a match); it can be turned off in *Options*
- **Ghost options:** opacity (100 / 80 / 50 / 25 % or hidden) and showing or hiding the names above the ghosts
- **Play again** button in the results window (marks you ready for the next match)
- **Level leader:** the room creator can hand this role to another player; the leader picks the level, manages the
  queue and accepts or rejects suggestions (only the creator removes and bans players, changes modifiers and starts
  or ends the match)
- **Level suggestions:** any player can suggest levels (up to 3 each, 20 in the list); the host or the leader can
  *Play now*, *Queue it* or *Reject*

### Changed
- *Options* screen reorganized in two columns
- Player counts, rooms with more than 4 players, the level leader and the suggestions need the updated room servers;
  with an older server the app works as before

## 0.3.2 — 2026-11-11

One file only: the OBB is gone. Install the APK; nothing goes in `Android/obb` anymore.

### Changed
- **Single APK:** the game content is inside the APK (about 615 MiB), so there is no `.obb` to copy anymore
- The **Neo Cosmos DLC content is no longer shipped** in the port (it was inside the OBB of 0.3.0 and 0.3.1; about 130 MB less)

### Added
- Notice when a custom level uses Neo Cosmos DLC features, which are not part of the port: the level still plays, with those effects disabled (English, Portuguese and Korean)

## 0.3.1 — 2026-11-11

The OBB changed in this version: install the new APK **and** replace the `.obb`.

### Added
- Room password (optional): set when creating a room, typed when joining a locked room; rooms with a password are marked in the list
- Host tools: **Ban** a player (by IP, while the room exists), besides *Remove*
- **Report** button next to other players' names (the room server logs it; the host is notified)
- Chat anti-spam: limit on how fast messages can be sent
- Optional swear-word filter for the chat and player names (Options screen, on by default)

### Fixed
- Empty level list after coming back from a match (the level selector can reopen in a featured category with only the official levels)
- A level download that receives no data for 30 s now fails with a message instead of staying at "Downloading 0%"
- Touches on the online screens going through to the level selector behind them, which could enter a level by itself

## 0.3.0 — 2026-11-10

### Added
- Level queue in rooms: the host lines up up to 8 levels
- New level picker: artwork, title, artist and author, *Workshop* / *Local* tag, search, filters and counter
- Options screen: language, main and fallback server
- Keyboard and controller navigation in the online screens

### Changed
- Room screen reorganized in groups ("Level" and "Modifiers")
- Level picker buttons resized to match the stone button art
- *Workshop* / *Local* tag is now translated

### Fixed
- Texts flashing in Portuguese for one frame before showing the selected language
- Empty level list when the level folders had not been read yet

## 0.2.0 — 2026-11-09

### Added
- Online rooms on the public server: public rooms by region and private rooms with a code
- Spectator mode: join a match in progress, or keep watching after finishing
- Room chat
- Host modifiers: Immortal and Speed (0.5x–2x)
- Levels that are not on ADOFAI.gg / TUF are sent to the room automatically (kept for 10 minutes)
- Screens in English, Portuguese and Korean, following the game language
- Optional check that the original game is installed from Google Play (build setting, off by default)

### Changed
- Matches start at the time set by the server and restart on their own after a fail
- Level browser texts are translated

## 0.1.0 — 2026-11-08

First Android build.

### Added
- Android build: ARM64, IL2CPP, Vulkan / OpenGL ES 3, landscape, own package name
- Custom levels without Steam Workshop: local level folder on the device
- Level import with the native Android file picker, including zips with Korean file names
- "Download Levels" button: level browser for ADOFAI.gg and TUF
- Touch scrolling in the level selector; larger selector on phones
- On-screen pause button
- App icon and name; no Unity splash screen
- Online portal in the main menu and first version of the online rooms

### Fixed
- Simultaneous level events ran in a different order than in the original game, which left a decoration on screen in some levels
- Desktop keyboard hook disabled on Android
