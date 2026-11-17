<p align="center">
  <img src="images/icon.png" width="96" alt="Sticky Notes icon">
</p>

<h1 align="center">Sticky Notes</h1>

<p align="center">
  Colourful paper notes you can write on and stick to any block face.<br>
  For Fabric and NeoForge.
</p>

<!-- header:start -->
![Version 1.0.0](https://img.shields.io/badge/version-1.0.0-6EC4A0?style=flat-square) ![Minecraft 1.21.1 | 1.21.11 | 26.3](https://img.shields.io/badge/Minecraft-1.21.1%20%7C%201.21.11%20%7C%2026.3-62B47A?style=flat-square) ![Fabric](https://img.shields.io/badge/Fabric-DBD0B4?style=flat-square) ![NeoForge](https://img.shields.io/badge/NeoForge-F16436?style=flat-square) [![Modrinth downloads](https://img.shields.io/modrinth/dt/sticky-notes?style=flat-square&logo=modrinth&label=Modrinth&color=1BD96A)](https://modrinth.com/mod/sticky-notes) [![CurseForge downloads](https://img.shields.io/curseforge/dt/CURSEFORGE_PROJECT_ID?style=flat-square&logo=curseforge&label=CurseForge&color=F16436)](https://www.curseforge.com/minecraft/mc-mods/sticky-notes) [![GitHub downloads](https://img.shields.io/github/downloads/CptGummiball/StickyNotes/total?style=flat-square&logo=github&label=GitHub)](https://github.com/CptGummiball/StickyNotes/releases)

*   [Wiki](https://github.com/CptGummiball/StickyNotes/wiki)
*   [Supported versions](https://github.com/CptGummiball/StickyNotes/wiki/Supported-Versions)
*   [Report a bug](https://github.com/CptGummiball/StickyNotes/issues/new/choose)
*   [Request a Minecraft version](https://github.com/CptGummiball/StickyNotes/issues/new?template=version_request.yml)
*   [API for mod developers](https://github.com/CptGummiball/StickyNotes/blob/main/api/README.md)
<!-- header:end -->

This repository holds the documentation, the [wiki](../../wiki), the [issue tracker](../../issues)
and the [API for mod developers](api/README.md). The mod itself is downloaded from Modrinth or
CurseForge. Sticky Notes is not open source; see [License](#license).

## What Sticky Notes is

* **Notes on block surfaces, not blocks:** paper notes sit flat on walls, floors, ceilings, chests and
  doors – up to four per block face, no collisions, no block space used.
* **A click on a note opens the note,** not the chest or door behind it.
* **An editor of its own:** a large sheet in the note's colour with paper grain and a folded corner,
  multi-line editing with selection, clipboard and word wrap – no recoloured sign screen.
* **16 colours and mixes:** dye with one dye, or mix two – yellow + blue gives green.
* **Owners and locks:** everybody reads every note; locked notes are edited only by their owner, and
  only the owner removes a note. Every action is checked by the server.
* **Persistent and tidy:** notes are saved with their chunk; a broken support block drops the note as an
  item that keeps text, colour, owner and lock.

## Works with other mods

Sticky Notes needs only Fabric API (Fabric) or nothing else (NeoForge). Notes are stored in the
loaders' chunk data attachments and drawn with the vanilla render pipeline, so they do not conflict
with block or entity mods. Players without the mod see no notes. Known limits: notes do not move with
pistons or doors (they drop as items), and world editors that bypass block updates are noticed only
when the chunk loads again.

## Version status

| Minecraft | Fabric jar | NeoForge jar |
|---|---|---|
| 1.21.1 | `stickynotes-1.0.0+mc1.21.1-fabric.jar` | `stickynotes-1.0.0+mc1.21.1-neoforge.jar` |
| 1.21.11 | `stickynotes-1.0.0+mc1.21.11-fabric.jar` | `stickynotes-1.0.0+mc1.21.11-neoforge.jar` |
| 26.3 | `stickynotes-1.0.0+mc26.3-fabric.jar` | `stickynotes-1.0.0+mc26.3-neoforge.jar` |

"Tested" means, for every listed version: client and dedicated server started, all automated game
tests passed, and the core flows were played in a real client. The exact loader versions are listed in
the wiki under [Supported Versions](../../wiki/Supported-Versions).

## Performance

One rough measurement in a development client (854×480 window, VSync off): 804 notes in view drew at
about 281 FPS against about 475 FPS for the same view without notes. Readings vary a lot between runs;
this is an order of magnitude, not a promise for every computer.

## Downloads

[Modrinth](https://modrinth.com/mod/sticky-notes)
[CurseForge](https://www.curseforge.com/minecraft/mc-mods/sticky-notes)

Please download Sticky Notes only from these pages. Pick the file whose name contains your
Minecraft version, for your loader.

## Reporting bugs

Please open an [issue](../../issues/new/choose) with the Minecraft version, the loader and its
version, the jar name, the other mods involved, and `logs/latest.log` (plus a crash report if
there is one).

## License

Sticky Notes is **not open source**. All rights reserved by cptgummiball; see [`LICENSE`](LICENSE).
In short:

* You may play with Sticky Notes, use it on any server and show it in videos and streams.
* You may put Sticky Notes into **modpacks**, as long as the jar files stay exactly as published.
* You may **not** modify, decompile, re-upload or otherwise redistribute Sticky Notes, or use its
  assets elsewhere.
* Mod developers may compile against the [Sticky Notes API](api/README.md).
* For anything else, open a [permission request](../../issues/new?template=permission_request.yml).

Sticky Notes is made by **cptgummiball**. It is not an official Minecraft product and is not
associated with Mojang or Microsoft.
