# Ace Attorney Trilogy 3DS Animation Restoration

**Release: v3**

This patch adds Steam character artwork and animation frames to *Phoenix Wright: Ace Attorney Trilogy* for Nintendo 3DS.
It keeps the original 3DS backgrounds.
Some character files also keep the original artwork, including close-ups and Furio Tigre's cafe rear view.

**You can install v3 with the US, EU, or JP version of the game.**
All three versions use the same ZIP file.
The folder name must match the title ID of your game.

[Download the v3 ZIP](https://github.com/GrouchoGlasses42/ace-attorney-trilogy/releases/download/v3/Ace-Attorney-Trilogy-3DS-v3-LayeredFS.zip)

## Changes

- Steam character artwork in all three games.
- Additional animation frames for blinks and gestures.
- Repairs to Phoenix's face and Acro's lower body.
- A correction to Iris's open-eye pose.
- A complete blink sequence for Edgeworth.
- A return to the neutral pose in Jake Marshall's drinking sequence.
- Three blinks in Manfred von Karma's sequence.
- Original motion sequences for selected Edgeworth, Gumshoe, and Dr. Hotti animations, with the applicable Steam poses.
- Original 3DS backgrounds and close-up artwork.

v3 is a complete patch.
You do not need earlier patches.
The game data is the same as the checked v0.5.5 build.

## Requirements

- A Nintendo 3DS with Luma3DS.
- An installed US, EU, or JP copy of the game.
- An SD card with space for the patch.
- The **Enable game patching** option in Luma3DS.

## Game versions

| Game version | Title ID | Folder on the SD card |
| --- | --- | --- |
| US | `0004000000138F00` | `luma/titles/0004000000138F00/romfs/` |
| EU | `0004000000133300` | `luma/titles/0004000000133300/romfs/` |
| JP | `0004000000108800` | `luma/titles/0004000000108800/romfs/` |

The ZIP contains the US folder name.
For EU or JP, only the title folder name changes.
The two pack files stay the same.

## ZIP contents

```text
luma/
└── titles/
    └── 0004000000138F00/
        └── romfs/
            ├── pack.inc
            └── pack.dat
```

`pack.dat` contains the game assets.
`pack.inc` identifies the position and size of each asset.
The game requires both files from the same release.

## Download check

The SHA-256 value for the v3 ZIP is:

```text
08dfea695eeeabf942d7d37e818d037ef8a5c470c18f40dac44b816eb3f02907
```

## Installation

1. Download the v3 ZIP from the link above.
2. Extract the ZIP on your computer.
3. Find the title ID for your game in the table above.
4. For EU or JP, rename the included `0004000000138F00` folder to the applicable title ID.
5. Turn off the console.
6. Remove the SD card from the console.
7. Connect the SD card to your computer.
8. If an earlier patch is present, make a backup of its two pack files.
9. Copy the extracted `luma` folder to the root of the SD card.
10. If a file replacement message appears, replace both `pack.inc` and `pack.dat`.
11. Put the SD card in the console.
12. Hold SELECT while you turn on the console.
13. Select **Enable game patching** in the Luma3DS menu.
14. Press START to save the setting.
15. Start the game.

If you installed this project's earlier companion update, remove that custom update before you use v3.
That update uses a different file path for the game assets.

## Removal

1. Turn off the console.
2. Connect its SD card to your computer.
3. Remove this release's `pack.inc` from the applicable `romfs` folder.
4. Remove this release's `pack.dat` from the same folder.

The game then uses its installed assets.
These steps do not remove your save data.

## Checks and limits

File checks cover 414 character files and 1,582 animation slots.
All pose references from the previous build remain in use.
The original backgrounds and story scripts remain unchanged from the previous build.

The checks include US game data and comparisons with applicable EU data.
This project has not compared a JP game dump.
The JP title ID above gives the installation path for that version.

This build has not had a full gameplay test on a console or an emulator in this project.
File checks do not confirm every scene during gameplay.

## Problems

[Open an issue](https://github.com/GrouchoGlasses42/ace-attorney-trilogy/issues/new).
Include the game version, case, scene, and a description of the problem.
If possible, include a screenshot.

## Credits

Capcom owns the game and the original artwork.

[Akoi89's Steam Enhanced project](https://github.com/Akoi89/aat-3ds-steam-enhanced) supplied artwork for the Phoenix and Acro repairs.
The project author also helped compare the animation files.

GrouchoGlasses42 maintains this release.
This is an unofficial patch.
