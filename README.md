# Gwent Card Forge

**Version 3.00 for Windows x64 · by [shafiaymaan](https://github.com/shafiaymaan)**

[Download the Windows app](https://github.com/shafiaymaan/gwent-card-forge-releases/releases/latest)

Edit Witcher 3 Gwent card pictures, English names and flavour descriptions. Create a new mod ZIP from the original cards, or open an installed Gwent mod and save changes directly into its folder. Compare the game original on the left with the mod and your changes on the right.

## Install

1. Open the latest release and download **GwentCardForge-3.00-Windows.zip** under **Assets**.
2. Extract the entire ZIP to a **new writable folder**. Copy your existing **data** folder into the new **GwentCardForge** folder if you want to reuse a local import.
3. Run **GwentCardForge.exe**. Keep **_internal** beside it. No separate Python installation is required.
4. If needed, click **Load game** and select your local Witcher 3 installation to import original card data.

The application is unsigned. Compare the ZIP checksum with **SHA256SUMS-3.00.txt** on the release page. Packaging checks do not guarantee acceptance by every antivirus or by Nexus Mods.

GitHub also generates **Source code (zip)** and **Source code (tar.gz)** links. These contain only this repository's documentation. Download the **Windows.zip** asset for the app.

## Edit an installed mod — new in 3.00

1. Click **Open mod** and choose a Gwent mod folder such as **The Witcher 3/Mods/modCustomGwentCards**, its **content** folder, or choose the game/Mods folder and select a mod.
2. Only cards represented by that mod's recognized artwork or English card text appear. The left panel shows the game original; the right starts with the mod's current artwork and text.
3. Change the picture, name and/or description, then **Queue this card** before switching cards. **Reset card** and **Use mod picture** return to the loaded mod baseline.
4. Close the game, then click **Save to mod** to update that same folder.
5. Use **All cards** to return to creating a new mod ZIP.

Each save creates a timestamped **.gwent-forge-backups** folder inside the selected mod, outside **content**. It contains the exact originals of changed files, restoration instructions and a record of newly created files. Other textures, strings, languages and files are preserved. The app rejects externally changed mod contents and restores replaced files if a save fails.

Mod-folder projects embed new pictures and queued edits. Open the matching mod before opening its project. Save a new project after updating a mod to continue from the new baseline. Existing original-card projects still open in **All cards** mode.

Supported inputs: version 6/7 single-mip **texture.cache**, recognized loose PNGs under original game-relative paths, and English **en.w3strings** versions 162/164. Bundled-only artwork, script/XML custom cards and non-English text are not editable in this mode. Shared changes affecting a card outside the loaded mod are rejected. Vortex redeployment may replace direct edits; keep your project and backups.

## Create a new mod

In **All cards**, choose a card, edit its picture, name and/or description, then **Queue this card**. Save a project or click **Forge ZIP**. Close the game and copy the exported **mods** folder into the game installation. Replace older **modCustomGwentCards** versions completely and disable conflicting card mods.

Power, faction and ability rules stay unchanged. Importing original game data reads game files without changing them. Artwork is imported locally; extracted card data, personal pictures and saved projects are excluded from the public download.

## Desktop features and validation

- Native Qt interface with a Witcher background, translucent panels, icons and short card transitions.
- Cached card previews and reduced background redraw work.
- Background imports, project operations, mod loading and saves.
- Portable Windows executable with its own runtime.
- Build details in **BUILD-INFO.json**, distributed-file checksums in **FILES.sha256**, and review information in **SECURITY.txt**.

Version 3.00 passed **30 automated tests**, packaged-app checks on Windows with **226 original/alternate previews across 216 card entries**, and an edit/save preservation check on a copy of an installed Gwent mod. The installed game mod was unchanged during validation. Validated original data: Witcher 3 Remastered v5.01. Test your edited mod in your game.

## Distribution and ownership

This is the official **downloads and documentation** repository. Application source is private. Downloading does not grant permission to rehost, resell, rebrand or claim authorship of the application. Please link to the official release page when sharing it.

Copyright © 2026 shafiaymaan. Free for personal, non-commercial use under [LICENSE.txt](LICENSE.txt). The license preserves rights granted by third-party licenses, including replacement of dynamically linked LGPL libraries. These restrictions do not claim ownership of your card projects or exported mods.

Qt, PySide6, Shiboken, Python, Pillow and other bundled components retain their respective licenses; notices and Qt source information are included in **_internal/THIRD-PARTY**. Witcher artwork and trademarks belong to CD PROJEKT RED and their respective owners. This is an unofficial tool, not affiliated with or endorsed by CD PROJEKT RED.
