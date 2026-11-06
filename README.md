# The Comet Store

This repository is the **Comet Store's online catalogue**. Comet's Store
(Orbit -> Store) reads `catalog.txt` from here, so an app added here appears
in every Comet without Comet changing at all.

* `catalog.txt` - every app: its name, version, price, where to download it,
  its SHA-256 (Comet checks it before installing), icon and screenshots.
* `apps/` - the programs. `icons/` - square PNG icons. `shots/` - screenshots.

## Adding an app

1. Put the program in `apps/`, a square PNG in `icons/`, screenshots in `shots/`.
2. Add a block to `catalog.txt` (copy one that is already there).
   `download` can also be a full `https://` address anywhere on the internet.
3. Only list programs whose licence allows them to be given out
   (MIT, BSD, Apache, public domain...), or that you made yourself.

Paid apps are **test mode** for now: no money moves.

Lua is MIT-licensed (see `LUA-LICENCE.TXT`), and so are Python - MicroPython (see `PYTHON-LICENCE.TXT`), jq (see `JQ-LICENCE.TXT`) and JavaScript - QuickJS (see `QJS-LICENCE.TXT`). SQLite is in the public domain.
2048, Snake, Mines, Sudoku, Guess the Number and Hello Windows were made for Comet (MIT).
Brick Breaker, Block Drop, Sky Defenders, Rock Blaster and Floppy are raylib-games classics (zlib - see `GAMES-LICENCE.TXT`).
