# Cutechess++ — A Cutechess Fork

*Summary of changes and additional features*

> **Read it here, or download it:** [Download this summary as a Word document (DOCX)](https://github.com/keith1760/Cutechess-plus-plus/raw/main/docs/Cutechess%2B%2BFork%20Summary.docx) · [Back to the main page](../README.md)

This document summarises the changes made in this fork of Cutechess. The additions focus on engine-versus-engine play, tournament and opening-book control, board presentation, configuration management and general usability.

**1. Pause engine-versus-engine matches**

> Engine-versus-engine matches can now be paused. The control is located at the upper-right of the main window.

**2. Explore alternative moves and variations during a match**

> During an engine-versus-engine match, the user can choose an alternative move and have the engines continue from that position.
>
> **Additional detail:** *The original game position can be restored at any time. Variations can be explored from other variations, allowing branches within branches to be tested. The time available to each engine for a move in a branch is set under Settings → Games → Branch Time per Move.*

**3. Filter UCI instructions**

> An optional filter allows only UCI instructions recognised by the GUI to be passed on.
>
> **Additional detail:** *This is intended to improve compatibility with engines that send newer or unfamiliar UCI instructions, which might otherwise prevent an engine from loading correctly. The filter can be enabled or disabled under Settings → General.*

**4. Customise the board and its appearance**

> Settings → General now includes controls for the background colour, board-square colours, main-board size and piece colours.
>
> **Additional detail:** *The General settings page is longer as a result, but it scrolls when necessary.*

**5. Display the opening name prominently**

> The name of the current opening is displayed prominently in the main window.

**6. Display the participating engines prominently**

> The names of the engines currently playing are displayed prominently.

**7. Make match scores and Elo differences easier to see**

> The current match score and the Elo difference implied by that score are displayed prominently.

**8. Optional bold text**

> An option to display bold text throughout the interface has been added. It can be switched on or off under Settings → General.

**9. Keep a named engine at the top of the board**

> An option keeps the selected named engine playing from the bottom of the board. The setting is available under Settings → General.

**10. Add a position-evaluation bar**

> A position-evaluation bar is now displayed.
>
> **Additional detail:** *Its light and dark sections automatically follow the colours of the pieces at the top and bottom of the board.*

**11. Show opening-book moves one at a time**

> Book moves can be displayed individually, with a user-defined pause between moves.
>
> **Additional detail:** *This makes it possible to watch how a starting position develops from a .bin or .pgn opening source, rather than having the completed position appear immediately. The pause is adjusted with a slider under Settings → Tournaments.*

**12. Save and restore configurations**

> The Tools menu now includes options to save a configuration and restore it later.

**13. Improve access to controls in smaller windows**

> Windows scroll bars have been added where needed so that settings and buttons remain accessible when they would otherwise fall outside the visible area.

**14. Adjust randomness in opening-book selection**

> A randomness slider has been added to the Tournament menu to provide control over opening-book move selection.
>
> **Additional detail:** *The interaction between the Polyglot code and Cutechess's own code appears to affect randomness in some circumstances. I did not fully identify the underlying cause. The slider provides a practical adjustment: zero is closest to the original settings. Pgn files work well and a collection of over 78000 pgn files is available for download. They are limited to 20 ply in length and are from games played by very strong players from the 21<sup>st</sup>, 20<sup>th</sup> and 19<sup>th</sup> centuries. I obtained them from *<https://www.pgnmentor.com/files.html> *I thank the publisher for making them available.*

**15. Remove the bottom slider**

> The slider at the bottom of the main window has been removed. Its functions are now available through buttons at the upper-right of the window.

**16. Save engine-versus-engine games as PGN**

> Engine-versus-engine games can be saved to a PGN file. This feature can be switched on or off in the New Tournament menu.

**17. Have each engine play both sides**

> An option allows each engine to play both sides of a starting position in an engine-versus-engine match. The setting is available in the Tournament menu.

**18. Show or hide board coordinates**

> A control has been added to show or hide the rank and file labels around the board (a–h and 1–8). The switch is under Settings → General.
>
> **Additional detail:** *Hiding the labels allows the board to be displayed significantly larger.*

**19. Bug fixes and general improvements**

> A number of bugs have been fixed, mainly involving window geometry and the persistence of settings.
>
> **Additional detail:** *AI tools, Claude and ChatGPT, were used extensively to add features and identify and implement fixes. Most changes addressed underlying causes rather than symptoms. Where an issue could not be resolved in that way, I specified more localised workarounds to address the observed behaviour.*

*There is a copy of the source code both inside the Linux appimage and the folder that contains the Win 11 executable and its dependencies.*

*Linux (AppImage): the main one of these is built on Ubuntu 24.04 (Qt 6.4.2, glibc 2.39), so it needs a distribution with glibc 2.39 or newer. Ubuntu 22.04 is too old. On Ubuntu 24.04 you may need to install FUSE 2 (`sudo apt install libfuse2t64`) or run the AppImage with `--appimage-extract-and-run`.*

*I have also made available a folder containing a version that should run on Linux as early as Mint 19 and Ubuntu 18, from 2018. It has not been tested on those but it loads correctly on Mint 22. It is very nearly but not quite the latest binary.*

*Windows: built with Qt 6.8.3 and should run on Windows 10 (1809 or later) and Windows 11. The coloured title bars only appear on Windows 11.*

*Most but not all changes that affect UCI engines should work with Winboard engines but I have not tested Winboard engines in this fork.*

*I would like to express my gratitude to the original programmers, without whose work this fork would not have been made.*
