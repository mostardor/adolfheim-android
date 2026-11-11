# Build information

Technical data of the port's builds. The build files themselves are not in this repository.
**Português:** os dados técnicos das builds do port. Os arquivos das builds não estão neste repositório.

## Settings (all versions)

| Item | Value |
|---|---|
| Engine | Unity 6000.3.27f2 (the original game uses 6000.3.25f1) |
| Package name | `com.adofaiport.personal` (does not replace the official app) |
| Scripting backend | IL2CPP, minimal managed stripping |
| Architecture | ARM64 (arm64-v8a) |
| Minimum Android | 8.0 (API 26) |
| Graphics APIs | Vulkan, then OpenGL ES 3 |
| Orientation | Landscape (both sides) |
| Packaging | APK + OBB (split application binary) |
| Unity splash screen | Off |
| Original-game check | Optional build setting (`ADOFAI_REQUIRE_OFFICIAL`) |

Level folder on the device: `Android/data/com.adofaiport.personal/files/Worlds`.

## Builds

### 0.3.0 — 2026-11-10

| File | Size | SHA-256 |
|---|---|---|
| APK | 81,598,737 bytes (77.8 MiB) | `b14f9fdae7e5b877e255db8afef38f604d120d8d3d4993a207a83b533812e0b6` |
| OBB | 686,059,738 bytes (654.3 MiB) | `fc97835b31e7706f10697cbd071b6f3b5ed2cdbd5c7483405c8e4e4be53f401d` |

- Original-game check: off
- Tested on: POCO F7
- The OBB content did not change since 0.2.0 (built on 2026-11-09)

### 0.2.0 — 2026-11-09

- Sizes and checksums were not recorded
- Tested on: POCO F7

### 0.1.0 — 2026-11-08

- APK about 80 MB, OBB about 686 MB; checksums were not recorded
- First build takes about 12 minutes (IL2CPP compiles about 8,400 C++ files)
- Tested on: POCO F7

## Notes on the port

- Shaders: the game's shaders were rebuilt for Android with `#pragma target 3.5` (OpenGL ES 3 has no Shader Model
  4.0). The four `Framebuffer` blend-mode shaders are approximations.
- Timing: simultaneous level events are ordered with a 10 µs tolerance, so IL2CPP/ARM64 keeps the same order as the
  original game.
- Input: the desktop keyboard hook is disabled on Android; touch uses the game's own mobile input path.
- Rendering: the world is drawn to a render texture with an adjustable scale; the UI stays at native resolution.
