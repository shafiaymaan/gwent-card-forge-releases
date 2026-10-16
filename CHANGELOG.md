# Release notes

## 2.00 — 2026-10-17

- Replaced the Tkinter wallpaper implementation with a native Qt interface.
- Added translucent panels, a wolf emblem, icon buttons and animated card previews.
- Restored visible original/custom card images and added a bounded image cache.
- Added background workers for imports, projects and ZIP exports.
- Added a portable Windows EXE build, resource discovery and rendered-preview tests.
- Fixed GUI resource cleanup so the application exits cleanly after rendering.
- Added author credit, Windows version information and application license notices.
- Published a public Windows download while keeping application source private.

## 1.00

Initial release of Gwent Card Forge.

- Import original card artwork, English names and descriptions from a local game installation.
- Compare original cards with edited pictures, names and descriptions side by side.
- Save portable projects with embedded pictures.
- Export and verify a complete installable mod ZIP containing selected changes.
- Keep extracted game data, personal pictures and generated mods outside version control.

Validated against Witcher 3 Remastered v5.01, with 216 card entries representing 228 game definitions and 226 artwork images. Includes automated source tests on Python 3.11 and 3.13.
