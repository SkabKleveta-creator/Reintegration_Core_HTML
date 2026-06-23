# Reintegration Core — District 01

## Current Build: v1.18.6 — Shaft + Health Shower Recovery

### BLUF

`v1.18.6` is the current working build for **Reintegration Core — District 01**. It extends the v1.18.5 playability recovery baseline by adding one new upward traversal room, `R07`, built around broken ladder segments, fixed-anchor grappling, and a Health Shower recovery interaction.

This build should be treated as **mechanically checked but still pending live phone playtest**.

---

## Current Design Locks

Do not change these without a deliberate version bump:

* No jump
* No boost
* Fixed-anchor grapple only
* 64×20 logical rooms
* 32×20 visible corridor
* Phone browser priority
* Vertical page scrolling allowed
* Door-driven validation
* Intent Log/tabletop panel hidden from live playable UI, not destructively removed
* Ladder/access rhythm preserved from v1.18.3 recovery base
* Glyphs may be next to ladders, but never on or vertically over ladder columns

---

## Current Room Flow

Current District 01 route:

`R02 → R03 → R12 → R04 → R05 → R06 → R07 → COMPLETE`

### R07 — Vertical Shaft

`R07` is an upward movement room designed to test vertical access without adding jump or boost.

Core purpose:

* Demonstrates upward movement through a shaft
* Uses broken ladder segments to create partial access, not full ladder solutions
* Requires fixed-anchor grappling to continue upward
* Preserves the access doctrine: authored anchors, readable routes, no arbitrary wall attachment
* Validates when Eli reaches the upper shaft exit platform

---

## New Mechanic: Health Shower

`v1.18.6` adds a Health Shower recovery point.

### Behavior

The Health Shower appears as a wall-mounted shower faucet tile.

When Eli activates it:

1. Eli stands in front of the shower.
2. The curtain closes.
3. Eli is hidden behind the curtain.
4. The shower visibly runs.
5. Player input is temporarily locked.
6. When the recovery cycle completes, Eli’s Stability restores to full.

### Recovery Result

* Stability restores to `3`
* The shower does not add combat, inventory, or health-pack logic
* It functions as a readable environmental recovery station

Player-facing intent:

> Recovery is part of the system, not a reward crate.

---

## v1.18.6 Change Summary

Added:

* New room `R07`
* Upward shaft traversal
* Broken ladder route structure
* Additional fixed grapple anchors for shaft movement
* Health Shower tile and interaction
* Curtain-hidden shower recovery animation
* R07 validation condition tied to reaching the upper shaft platform
* R07 glyphs and dialogue
* R06 route extension into R07
* R07 completion route to District Complete

Corrected during check:

* R07 grapple landing points were moved off ladder columns and onto valid adjacent platform positions
* Glyph placement was checked against ladder-column rules
* Glyph text keys were checked against visible glyph positions
* Sync/relay logic from v1.18.5 remains preserved

---

## Acceptance Checks Completed

The following checks passed before this README update:

* All rooms remain 64×20 logical size
* Visible corridor remains 32×20
* R06 transitions into R07
* R07 loads successfully
* R07 high exit completes the district
* R07 shaft route is mechanically traversable
* Health Shower activates
* Curtain closes during shower recovery
* Eli is hidden during shower recovery
* Stability restores to full after shower completion
* R07 validates only after reaching the upper shaft platform
* No glyphs are placed on ladder tiles
* No glyphs are vertically over ladder columns
* All visible glyphs have matching dialogue text
* No orphan glyph dialogue keys were detected

---

## Known Testing Status

### Passed

* Boot-level recovery checks
* Desktop smoke checks
* Mobile-layout smoke checks
* R02 → R03 route recovery
* R03 relay/SYNC recovery
* Glyph/ladder placement checks
* R07 assisted traversal check
* Health Shower recovery check

### Still Required

Live playtest on actual phone browser:

* Touch control comfort
* Shaft readability
* Grapple timing feel
* Whether the broken ladder route is obvious enough
* Whether the Health Shower interaction is discoverable
* Whether vertical scrolling and mobile controls remain comfortable during R07

---

## Current Development Rule

Do not tune visuals, expand mechanics, or add another room until the v1.18.6 phone playtest confirms:

1. Eli can move comfortably on phone.
2. Grapple access works without fighting the controls.
3. The upward shaft is readable.
4. The Health Shower is understandable.
5. The district can still be completed from R02 through R07.

---

## Build Doctrine

This build is not a platformer expansion.

It remains a systems-repair traversal prototype where Eli observes, routes, stabilizes, validates, and moves through authored access points.

The grapple is not a movement toy.
The ladder is not a decorative tile.
The shower is not a pickup.
The door is still the proof gate.
