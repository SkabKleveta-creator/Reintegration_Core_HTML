# BLACKBOX SQUADRON

**BLACKBOX SQUADRON** is a browser-based vertical arcade shooter prototype built as a single-file HTML/CSS/JavaScript game.

It is rough, playable, and intentionally built as a fast AI-assisted prototype: move, shoot, dodge, bomb, survive, and keep pushing into the next wave.

## Play the live prototype

**Live demo:**
https://skabkleveta-creator.github.io/BLACKBOX_SQUADRON/

## Current build

**Version:** `v0.1.4`
**Status:** Public playable prototype
**Platform:** Browser / GitHub Pages
**Architecture:** Single-file HTML game, no external libraries, no external assets

## What is included

* Vertical scrolling arcade shooter gameplay
* Keyboard controls
* Touch controls for mobile
* Player movement, firing, bombs, lives, score, and high score
* Enemy waves with multiple basic enemy behaviors
* Enemy bullets and collision detection
* Spread Shot pickup
* Falling obstacle/debris system
* Level progression
* Particle explosions and screen shake
* Mobile-safe layout for phone testing
* GitHub Pages deployment

## Controls

### Desktop

| Action        | Control           |
| ------------- | ----------------- |
| Move          | Arrow keys / WASD |
| Fire          | Space             |
| Bomb          | C                 |
| Start / Pause | Enter             |
| Restart       | R                 |

### Mobile

| Action        | Control         |
| ------------- | --------------- |
| Move          | On-screen D-pad |
| Fire          | FIRE button     |
| Bomb          | BOMB button     |
| Start / Pause | START button    |
| Restart       | RST button      |

## Known limitations

This is an early prototype, not a finished game.

Current limitations:

* Power-ups are still limited, with Spread Shot as the primary pickup.
* Health / repair pickups are not implemented yet.
* Bomb restore pickups are not implemented yet.
* Shield, rapid fire, rail shot, and drone wing pickups are planned.
* There is no boss system yet.
* The level director / randomizer is planned for the next major patch.
* Mobile controls work, but still need feel-testing across different phones.
* Balance is intentionally rough while the core loop is being built.

## Next planned patch: v0.2

The next planned patch focuses on the reward loop and replayability.

Planned v0.2 additions:

* Expanded power-up table
* Health / repair pickups
* Bomb pickups
* Shield pickup
* Rapid fire pickup
* Rail shot pickup
* Drone wing pickup
* Weighted drop logic
* Procedural level director / randomizer
* Difficulty bands
* Level modifiers

See:

```text
docs/NEXT_PATCH_V0.2_POWERUPS_LEVEL_DIRECTOR.md
```

## Project goal

The goal is to see how far a lightweight, browser-based arcade game can be pushed using AI-assisted prototyping without requiring a new game engine, build system, or asset pipeline.

The current development lane is:

```text
Single HTML file → GitHub repo → GitHub Pages → playable public prototype
```

## Repository structure

```text
BLACKBOX_SQUADRON/
  index.html
  blackbox-squadron-v0.1.4.html
  README.md
  docs/
    GITHUB_UPLOAD_CHECKLIST.md
    NEXT_PATCH_V0.2_POWERUPS_LEVEL_DIRECTOR.md
    PATCH_LOG.md
    PROJECT_STATUS.md
```

## Development notes

This project is being built in small, controlled patches.

The current baseline should be protected before major changes. Future updates should preserve:

* Single-file browser compatibility
* GitHub Pages deployment
* Keyboard controls
* Touch controls
* Existing obstacle system
* Current arcade feel
* Fast restart / quick play loop

## Release status

Current public prototype: **v0.1.4**

Recommended release label:

```text
BLACKBOX SQUADRON v0.1.4 — Public Prototype
```

This should be treated as a pre-release / prototype release, not a finished game.
