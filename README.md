# Gwent Card Forge

**Version 2.50 for Windows x64 · by [shafiaymaan](https://github.com/shafiaymaan)**

[Download the Windows app](https://github.com/shafiaymaan/gwent-card-forge-releases/releases/latest)

Edit the original Witcher 3 Gwent card pictures, English names and flavour descriptions, then export an installable mod ZIP. Compare the original card with your changes side by side. Save projects with your pictures embedded.

## Install

1. Open the latest release and download **GwentCardForge-2.50-Windows.zip** under **Assets**.
2. Extract the entire ZIP to a **new writable folder** on your PC. Do not merge it over a 2.00 installation, because that would leave the old nested library ZIP behind.
3. Open the **GwentCardForge** folder and run **GwentCardForge.exe**. Keep its **_internal** folder alongside it. No separate Python installation is needed.
4. Click **Load game** and select your local Witcher 3 installation to import original card data.

The application is unsigned. The official download is published only by **shafiaymaan** in this repository; use the release's **SHA256SUMS.txt** to compare the ZIP checksum.

GitHub also generates links named **Source code (zip)** and **Source code (tar.gz)**. Those contain only this repository's documentation, not the Windows app. Download the **Windows.zip** asset instead.

## Use

Choose a card, edit its picture, name and/or description, then click **Queue this card** before switching cards. Save your project or click **Forge mod ZIP**. Close the game and copy the exported **mods** folder into the game installation. Replace older **modCustomGwentCards** versions completely and disable conflicting card mods.

Power, faction and ability rules stay unchanged. The app reads original game files without changing them. Original card artwork is imported locally; extracted card data, personal pictures and projects are not included in the download.

## What's new in 2.50

- Removed the nested Python standard-library ZIP; its unchanged modules are included as individual files.
- Removed the unused Pillow/Tkinter bridge from the Qt application.
- Added verified dependency hashes, build details and a per-file SHA-256 inventory.
- Rebuilt in a fresh environment with hash-locked official PyPI wheels.

The [2.50 ZIP scan on VirusTotal](https://www.virustotal.com/gui/file/98819ca234724654fde9df93d60a154f3ba0a0702db7a0dabe07156b6450d515) showed no detections, including **Zillya: Undetected**, when checked on 20 October 2026. Microsoft Defender found no threats in the extracted application folder. VirusTotal warned that this large multi-file archive may not receive complete inner-file scanning; the main EXE was not separately submitted.

This addresses Nexus Mods' nested-archive restriction. The EXE remains unsigned and Nexus may still require moderator review. Read **SECURITY.txt** in the download and the scan results linked on the release page.

## Desktop features

- Native Qt interface with a Witcher background, translucent panels, icons and short card transitions.
- Restored card previews, cached pictures and reduced background redraw work.
- Background import, project operations and mod export.
- Portable Windows executable with its own runtime.

Validated with Witcher 3 Remastered v5.01, 216 card entries and 226 original/alternate artwork previews. The release passed 21 format, export and interface checks and packaged-app checks on Windows.

## Distribution and ownership

This is the official **downloads and documentation** repository. Application source is private. Downloading does not grant permission to rehost, resell, rebrand or claim authorship of the application. Please link to the official release page when sharing it.

Copyright © 2026 shafiaymaan. Free for personal, non-commercial use under [LICENSE.txt](LICENSE.txt). The license preserves the rights granted by third-party licenses, including replacement of dynamically linked LGPL libraries. These restrictions do not claim ownership of your card projects or exported mods.

Qt, PySide6, Shiboken, Python, Pillow and other bundled components retain their respective licenses; notices and Qt source information are included in **_internal/THIRD-PARTY**. The Witcher artwork and trademarks belong to CD PROJEKT RED and their respective owners. This is an unofficial tool, not affiliated with or endorsed by CD PROJEKT RED.
