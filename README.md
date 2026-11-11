# ADOFAI PC -> Android Port

Unofficial, fan-made Android port of **A Dance of Fire and Ice** (7th Beat Games), with custom levels and online
rooms on the phone.

> Not affiliated with, or endorsed by, 7th Beat Games. "A Dance of Fire and Ice" belongs to 7th Beat Games.

Support the developers: buy the game on [Google Play](https://play.google.com/store/apps/details?id=com.fizzd.connectedworlds)
or [Steam](https://store.steampowered.com/app/977950/A_Dance_of_Fire_and_Ice/).

## What the port adds

- **Custom levels on the phone:** local level folder, level import with the native file picker (`.zip` / `.adofai`),
  and a level browser for ADOFAI.gg and TUF that downloads and installs on the device
- **Touch:** tap to play, drag to scroll the level list, short tap to enter a level, on-screen pause button
- **Online rooms** (up to 4 players, public or private): race ghosts, spectator mode, chat, host modifiers
  (Immortal, Speed 0.5x–2x), level queue
- **Online portal** in the main menu
- Screens in English, Portuguese and Korean
- Larger, touch-friendly level selector; no Unity splash screen

## Versions

| Version | Date | Highlights |
|---|---|---|
| [0.3.0](releases/notes-0.3.0.md) | 2026-11-10 | Level queue, new level picker with artwork, options screen, text flicker fix |
| [0.2.0](releases/notes-0.2.0.md) | 2026-11-09 | Online rooms on the public server, spectator, chat, modifiers, EN/PT/KO |
| [0.1.0](releases/notes-0.1.0.md) | 2026-11-08 | First Android build, custom levels, level import and download |

Full list: [CHANGELOG.md](CHANGELOG.md). Technical data of each build (sizes, checksums, settings):
[docs/BUILD-INFO.md](docs/BUILD-INFO.md).

## Requirements

- Android 8.0 or newer (API 26+), 64-bit ARM (arm64-v8a)
- Vulkan or OpenGL ES 3
- About 800 MB of free storage, plus your levels
- Internet only for the level browser and the online rooms

## Known issues

- The four `Framebuffer` blend-mode shaders are approximations, so a few decorations can look different
- The Neo Cosmos DLC is not part of the port
- Controllers and very heavy levels are not well tested yet
- Tested on one device so far (POCO F7); reports from other devices are welcome

## Reporting a problem

Open an [issue](../../issues/new/choose) with your device, Android version, port version and, if it is a level,
its name or link.
---

## Português

Port não oficial, feito por fãs, de **A Dance of Fire and Ice** (7th Beat Games) para Android, com fases
personalizadas e salas online no celular.

> Sem vínculo com a 7th Beat Games nem endosso dela. "A Dance of Fire and Ice" pertence à 7th Beat Games.

Apoie os desenvolvedores: compre o jogo na [Google Play](https://play.google.com/store/apps/details?id=com.fizzd.connectedworlds)
ou na [Steam](https://store.steampowered.com/app/977950/A_Dance_of_Fire_and_Ice/).

### O que o port acrescenta

- **Fases personalizadas no celular:** pasta local de fases, importação pelo seletor de arquivos do Android
  (`.zip` / `.adofai`) e navegador do ADOFAI.gg e do TUF, que baixa e instala no aparelho
- **Toque:** tocar para jogar, arrastar para rolar a lista, toque curto para entrar na fase, botão de pausa na tela
- **Salas online** (até 4 jogadores, públicas ou privadas): fantasmas, espectador, chat, modificadores do anfitrião
  (Imortal, Velocidade 0,5x–2x) e fila de fases
- **Portal Online** no menu principal
- Telas em português, inglês e coreano
- Seletor de fases maior, próprio para toque; sem a abertura do Unity

### Versões

| Versão | Data | Destaques |
|---|---|---|
| [0.3.0](releases/notes-0.3.0.md) | 10/11/2026 | Fila de fases, seletor de fases com arte, tela de opções, correção dos textos piscando |
| [0.2.0](releases/notes-0.2.0.md) | 09/11/2026 | Salas online no servidor público, espectador, chat, modificadores, PT/EN/KO |
| [0.1.0](releases/notes-0.1.0.md) | 08/11/2026 | Primeira build Android, fases personalizadas, importar e baixar fases |

Lista completa: [CHANGELOG.md](CHANGELOG.md). Dados técnicos de cada build (tamanhos, checksums, configurações):
[docs/BUILD-INFO.md](docs/BUILD-INFO.md).

### Requisitos

- Android 8.0 ou mais novo (API 26+), ARM de 64 bits (arm64-v8a)
- Vulkan ou OpenGL ES 3
- Cerca de 800 MB livres, mais as suas fases
- Internet só para o navegador de fases e as salas online

### Problemas conhecidos

- Os quatro shaders `Framebuffer` dos modos de mistura são aproximações; algumas decorações podem ficar diferentes
- A DLC Neo Cosmos não faz parte do port
- Controles e fases muito pesadas ainda foram pouco testados
- Testado em um aparelho até agora (POCO F7); relatos de outros aparelhos são bem-vindos

### Relatar um problema

Abra uma [issue](../../issues/new/choose) com o aparelho, a versão do Android, a versão do port e, se for uma fase,
o nome ou o link dela.
