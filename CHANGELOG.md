# Changelog

Versions of the Android port. Dates are YYYY-MM-DD.

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
