# Cutechess++

[![DOWNLOAD CUTECHESS++](https://img.shields.io/badge/DOWNLOAD-CUTECHESS%2B%2B-brightgreen?style=for-the-badge)](https://github.com/keith1760/Cutechess-plus-plus/releases/latest)

**Cutechess++** is an unofficial fork of [Cute Chess](https://github.com/cutechess/cutechess), with additional features and changes developed independently. It is not endorsed by the original Cute Chess project.

## Latest release: 1.3

The current release provides builds for Linux and Windows, together with the source code.

### Downloads

- **Linux (modern systems):** [Cutechess++.AppImage](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess.AppImage)
- **Linux (older systems):** [Appimage for older versions of Linux](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess%2B%2B.Appimage)
- **Windows:** [Cutechess++Windows.zip](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess%2B%2BWindows.zip)
- **Source code:** [Cutechess++Sourcecode](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess%2B%2BSourcecode)

> [!WARNING]
> **Linux users: AppImages will not run until they are set to "Execute".**
> Downloaded files lose their execute permission, so the AppImage will do nothing (or report a permissions error) when you try to open it. Set the permission once, as follows:
>
> **From the terminal** (in the folder containing the download; use the file's actual name):
>
> ```
> chmod +x Cutechess++.AppImage
> ```
>
> **From the file manager:** right-click the AppImage → **Properties** → **Permissions** tab → tick **"Allow executing file as program"** (some systems say **"Is executable"**, or **"Execute"**) → close. Then double-click the file to run it.

## What is Cutechess++?

Cutechess++ builds on the original Cute Chess application, with additions intended to make engine matches and tournament play more flexible.

### Headline features

1. **Pause and resume engine-v-engine matches.** The board, clocks and game record stay unchanged, even if an engine has already started thinking or is about to return a move. It also works with human games and with tournaments running several games concurrently.
2. **Explore alternative moves during a match.** Pick a different move and the engines continue from that branch, so you can see what might have happened without losing the original game. Branches within branches are supported, and the original game can be restored and resumed at any time.
3. **Swiss tournaments.** A new format alongside the existing ones. Round 1 pairs by seed; later rounds pair within score groups, top half against bottom half, with floaters moving down. Nobody meets the same opponent twice unless unavoidable. With an odd number of players, the lowest-ranked player without a bye sits out each round, and the bye counts as a win. Standings include bye points. Also available in cutechess-cli with `-tournament swiss`.
4. **Tournament reports.** Cross tables and HTML reports, plus a Previous Tournaments window that saves reports automatically for later review.
5. **Resume an interrupted tournament from its existing PGN file.**

### Display and usability

6. Opening name, participating engines, scores and Elo differences shown prominently in engine-v-engine matches.
7. Customisable board: background, square and piece colours, and board size (indirectly).
8. Keep a chosen engine at the bottom (or top) of the board whichever colour it plays, so you can follow one engine's style without reorienting between games.
9. Colour-coordinated position-evaluation bar.
10. Scroll bars so controls stay reachable in small windows.
11. Save and restore configurations.

### Openings

12. Watch opening-book moves played one at a time (from a .bin or .pgn source) instead of the finished position appearing at once. The delay is configurable, and allows the watcher to see how the start position for the game developed. The pause between opening moves is independent of time limits.
13. Paired openings: each engine in turn plays both sides of the same opening.

### Engine compatibility

14. Optional filter that ignores UCI instructions that Cutechess doesn't recognise, to help with engines that send non-standard output. A "future-proofing" feature: new UCI instructions that a GUI does not recognise can cause crashes. This filters them out.

### General notes

A fuller account of the fork's changes is available in the [Cutechess++ fork summary (DOCX)](docs/Cutechess%2B%2B-Fork-Summary.md). It opens as a readable page here, and the page has a link to download the original Word (DOCX) file.

## Building from source

The source archive is intended for users who wish to inspect, build or modify the application.

- Cutechess++ uses **Qt 6**; the source build requires **Qt 6.8 or later**.
- The Linux AppImage packages its Qt runtime, so a separate Qt installation is not normally required to run that AppImage.
- The source archive includes the project's licence and notices. Please consult them before redistributing modified or unmodified versions.

## Project status

Cutechess++ is an independent fork. It is not an official release of, or endorsed by, the original Cute Chess project. The original project and its contributors are not responsible for this fork or its changes.
