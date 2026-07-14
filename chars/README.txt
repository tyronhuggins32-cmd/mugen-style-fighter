# New M.U.G.E.N Game

Pure DEF starter base for official Elecbyte M.U.G.E.N 1.0.

## Current scope

- Custom title screen and game-mode menu through `system.def`
- Empty roster and stage list through `select.def`
- No custom characters yet
- No engine modifications
- Reuses the stock M.U.G.E.N 1.0 system sprites, sounds, fonts, and fight UI

## Repository layout

```text
new-mugen/
├─ README.md
├─ data/
│  ├─ mugen.cfg.change.txt
│  └─ puredef/
│     ├─ system.def
│     └─ select.def
├─ chars/
│  └─ README.txt
├─ stages/
│  └─ README.txt
└─ sound/
   └─ README.txt
```

## Install into M.U.G.E.N

1. Copy the `data/puredef` folder into the `data` folder of an official M.U.G.E.N 1.0 installation.
2. Open the installation's existing `data/mugen.cfg`.
3. Find the `motif =` line under `[Options]`.
4. Change that line to:

```ini
motif = data/puredef/system.def
```

5. Keep the game resolution at `1280x720` while using this first motif base.
6. Start M.U.G.E.N.

## Current title-menu modes

- Arcade
- VS Mode
- Training
- Watch
- Exit

The modes are present now, but Arcade, VS, Training, and Watch need character entries before they can start a match.

## Adding content later

Characters will be created one at a time inside `chars/`. Each finished character will then be added to `data/puredef/select.def`.

Stages will be added inside `stages/` and registered in the same `select.def`.

## Important

This repository is an overlay. Do not upload or redistribute the official M.U.G.E.N executable or stock Elecbyte assets in this repository.
