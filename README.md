# Cutechess++

[![DOWNLOAD CUTECHESS++](https://img.shields.io/badge/DOWNLOAD-CUTECHESS%2B%2B-brightgreen?style=for-the-badge)](https://github.com/keith1760/Cutechess-plus-plus/releases/latest)

**Cutechess++** is an unofficial fork of [Cute Chess](https://github.com/cutechess/cutechess), with additional features and changes developed independently. It is not endorsed by the original Cute Chess project.

## Latest release: 1.3

The current release provides builds for Linux and Windows, together with the source code.

### Downloads

- **Linux (modern systems):** [Cutechess.AppImage](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess.AppImage)
- **Linux (older systems):** [Cutechess++.Appimage](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess%2B%2B.Appimage)
- **Windows:** [Cutechess++Windows.zip](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess%2B%2BWindows.zip)
- **Source code:** [Cutechess++Sourcecode](https://github.com/keith1760/Cutechess-plus-plus/releases/download/1.3/Cutechess%2B%2BSourcecode)

[View all releases](https://github.com/keith1760/Cutechess-plus-plus/releases)

## What is Cutechess++?

Cutechess++ builds on the original Cute Chess application, with additions intended to make engine matches and tournament play more flexible.

### Main additions and changes

This document summarises the changes made in this fork of Cutechess.

#### 1. Pause engine-versus-engine matches

Engine-versus-engine matches can now be paused and resumed.

The board, clocks and game record remain unchanged, even if an engine has already started thinking or is about to return a move. The facility also works with games involving human players and with tournaments running several games concurrently.

#### 2. Explore alternative moves and variations during a match

This facility is intended for examining what might have happened had an engine chosen a different move, without losing or altering the original game. During an engine-versus-engine match, the user can choose an alternative move and have the engines continue playing from that branch. Branches within branches can be played through by the engines. The original game can be restored and restarted at any time.

#### 3. Filter UCI instructions

An optional filter has been introduced to ignore UCI instructions from engines which are not recognised by Cutechess. It is enabled by default and can be switched off under Settings → General. It is intended to "future proof" the program.

#### 4. Introduce Swiss tournaments

A Swiss tournament format has been added alongside the existing tournament formats.

#### 5. Introduce tournament cross tables and reports

#### 6. Save and review previous tournaments

A new Previous Tournaments facility automatically saves tournament reports for later inspection.

#### 7. Resume an interrupted tournament from its existing PGN file

#### 8. Display the opening name prominently. Display the participating engines prominently. Display match scores and Elo differences

#### 9. Customise the board and its appearance

Users can choose colours of background, board squares, board size (indirectly) and piece colours.

#### 10. Keep a named engine at the top or bottom of the board

An option allows a selected engine to remain at the bottom of the board, irrespective of whether it is playing White or Black.

#### 11. Position-evaluation bar has been added

#### 12. Show opening-book moves one at a time in engine – engine matches

This makes it possible to watch how a starting position develops from a .bin or .pgn opening source, rather than having the completed position appear immediately.

#### 13. Save and restore configurations

#### 14. Improve access to controls in smaller windows by scroll bars

#### 15. Adjust randomness in opening-book selection

#### 16. Have each engine in turn play both sides of an opening during an engine – engine match

A fuller account of the fork's changes is available in the [Cutechess++ fork summary (DOCX)](https://github.com/keith1760/Cutechess-plus-plus/raw/master/docs/Cutechess%2B%2BFork%20Summary.docx).

## Building from source

The source archive is intended for users who wish to inspect, build or modify the application.

- Cutechess++ uses **Qt 6**; the source build requires **Qt 6.8 or later**.
- The Linux AppImage packages its Qt runtime, so a separate Qt installation is not normally required to run that AppImage.
- The source archive includes the project's licence and notices. Please consult them before redistributing modified or unmodified versions.

## Project status

Cutechess++ is an independent fork. It is not an official release of, or endorsed by, the original Cute Chess project. The original project and its contributors are not responsible for this fork or its changes.
