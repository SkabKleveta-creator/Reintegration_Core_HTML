# Reintegration Core — Isometric Arcade

## Current Build: v0.4.3 — Validation Feedback Pass

Playable page:

https://skabkleveta-creator.github.io/Reintegration_Core_HTML/

---

## BLUF

**Reintegration Core** is now an **isometric systems-repair arcade crawler**.

The game is no longer being developed as the old side-view traversal branch. It should continue as a phone-first, single-file HTML5 Canvas arcade prototype where Eli moves through authored isometric facility sectors, diagnoses system failures, uses bounded repair tools, validates each sector, and advances only when the route is actually proven.

Core doctrine:

> A system is not fixed because it looks fixed. It is fixed when the evidence validates.

Current maturity posture:

> `v0.4.3` is the current arcade candidate. It adds clearer validation feedback through a compact Proof Deck so the player can see what is still blocking sector validation before reaching the exit.

This build is **mechanically checked by static/code audit** and still needs live browser and phone playtesting.

---

## Current Direction

Reintegration Core should continue as:

* an isometric systems-repair arcade crawler
* a playable proof-of-repair engine
* a phone-first browser game
* a bounded-tool intervention game
* a validation-first progression prototype

It should **not** drift into:

* a generic platformer
* a shooter
* a TTRPG port
* a visual mockup / UI shell
* a lore-first worldbuilding project
* a traversal-upgrade game

---

## Current Sector Chain

The current isometric branch uses a 16-sector District 01 route:

`R02 → R03 → R12 → R04 → R05 → R06 → R07 → R08 → R09 → R10 → R11 → R20 → R21 → R22 → R23 → R13 → COMPLETE`

Current sector identities:

| Sector | Name | Primary Proof Theme |
|---|---|---|
| R02 | Ingress Utility Deck | Fault cleanup |
| R03 | Relay Channel | Relay confirmation |
| R12 | Scan Layer | Hidden route scanning |
| R04 | Thermal Intake | Heat stabilization |
| R05 | Catalyst Basin | Catalyst dampening |
| R06 | Fault Gallery | Faults + relays |
| R07 | Fault Recovery | Fault-line cleanup |
| R08 | Integration Gauntlet | Mixed failures + relays |
| R09 | Audit Mesh | Faults + scan + relays |
| R10 | Thermal Relay | Heat + relays |
| R11 | Catalyst Fork | Catalyst + faults + relays |
| R20 | Branch Junction | Fault cleanup in bay structure |
| R21 | Sealed Annex | Relay proof / locked annex |
| R22 | Long Causeway | Heat stabilization across distance |
| R23 | Convergence Hub | Mixed failures in open hub |
| R13 | Final Integration Corridor | Final all-system proof |

---

## Locked Posture

Do not change these without a deliberate version bump and explicit design decision:

* No HOOK
* No jump
* No boost
* No generic shooting
* No arbitrary traversal upgrade
* Tools are interventions, not weapons
* Doors validate proof before advancement
* Glyphs / evidence nodes preserve judgment
* Relays are confirmation nodes, not decoration
* Health Shower remains a recovery station
* Phone playability matters
* Keep the separate-room, validate-to-advance architecture unless explicitly ordered otherwise

Important correction:

> HOOK was removed by design. Do not reintroduce fixed-anchor grapple or anchor tiles unless a new branch explicitly authorizes it.

---

## Current Tool Doctrine

Tools are bounded interventions. They are not weapons.

| Tool | Purpose | Design Meaning |
|---|---|---|
| A / PULSE | Clears live fault tiles and stuns bots | Interrupt visible system corruption / pressure |
| B / SCAN | Reveals hidden route data | Find what the visible layer hides |
| B / SYNC | Confirms relay state | Confirmation must change real state |
| B / THERM | Cools heat / vent sources | Stabilize runaway system pressure |
| B / DAMP | Clears catalyst blocks | Reduce amplification / material obstruction |
| B / READ | Reads evidence / glyph nodes | Preserve interpretation and judgment |
| Y / USE | Interacts with doors, relays, showers, glyphs | Commit to evidence or attempt validation |
| R / TOOL+ | Rotates selected B-tool | Choose the correct intervention |

---

## Controls

### Mobile

* Floating left joystick: move Eli
* A: PULSE
* B: selected repair tool
* Y: interact / use / validate at exit
* R: rotate selected B-tool
* Tool tray: tap a tool to select it

### Keyboard

* WASD / arrow keys: move
* Space / Z / J: PULSE
* X / K: selected B-tool
* E / Y: interact / use
* R / Tab: rotate tool
* Enter / Escape: start / prompt current objective / restart after completion

---

## v0.4.3 Change Summary

Primary maturity target:

> Validation feedback pass.

Added:

* Compact Proof Deck below the HUD
* Live sector objective display
* Live validation blocker chips
* Next-action hint based on remaining proof blockers
* Failed validation messages that include the next proof action
* Immediate proof-state refresh after PULSE clears faults

Preserved:

* Isometric room architecture
* Separate-room sector chain
* Validate-to-advance flow
* No HOOK posture
* No jump / no boost
* Tool-as-intervention doctrine
* Health Shower recovery role
* Evidence/glyph role
* Relay proof role

---

## Current QA Status

### Static/code checks completed for v0.4.3

* JavaScript syntax check passed
* Runtime smoke test with mocked DOM/canvas passed
* Game start enters `PLAY` state
* Starts in `R02`
* 16-sector chain resolves to `COMPLETE`
* `ORDER` matches the sector chain
* All sectors are rectangular
* Every sector has one spawn `P`
* Every sector has one exit `E`
* Every sector has Health Shower `U`
* Every sector has evidence/glyph `G`
* Rule-required tiles exist per sector
* Exit remains reachable after required cleanup
* Faults / heat / catalyst / relays / glyphs / showers remain targetable
* `HOOK` string absent
* Anchor tile `A` absent from all maps
* Proof Deck functions are present

### Still required

Live browser and phone playtest:

* actual phone control comfort
* joystick feel
* tool tray usability
* Proof Deck vertical space on small screens
* whether NEXT hints help without over-handholding
* whether the 16-sector chain feels too long
* bot pressure and patrol feel
* sector readability under movement pressure
* final sector payoff
* complete start-to-finish win/restart flow in browser

Do not claim phone-tested until it has actually been played on a phone.

---

## Arcade Maturity Snapshot

| Category | Current Score | Notes |
|---|---:|---|
| Core loop clarity | 4 / 5 | Observe, repair, validate, advance is now clearer |
| Isometric map readability | 3 / 5 | Needs sector readability pass |
| Sector identity | 4 / 5 | Larger varied sectors are structurally distinct |
| Tool usefulness | 4 / 5 | Tools map to actual proof work |
| Validation clarity | 4 / 5 | Proof Deck improves blocker visibility |
| Evidence/glyph usefulness | 3 / 5 | Evidence exists but can matter more mechanically |
| Mobile control feel | 3 / 5 | UI exists, live phone feel unverified |
| Hazard/bot pressure | 3 / 5 | Needs tuning after playtest |
| Progression pacing | 3 / 5 | 16 sectors may be long |
| Win/restart flow | 4 / 5 | Mechanically present, live browser test required |
| Visual arcade polish | 3 / 5 | Functional isometric presentation, needs identity pass |
| Replayability / fun factor | 3 / 5 | Repair logic is sound; arcade tension needs tuning |

---

## Recommended Next Build Loop

Recommended next target:

> `v0.4.4 — Sector Readability Pass`

Focus:

* improve floor/wall separation
* improve hazard visibility
* improve relay visibility
* improve exit visibility
* improve glyph/evidence readability
* improve sector identity without changing validation logic

Do not change tools, sector chain, validation rules, or controls unless a readability failure requires it.

---

## Build Doctrine

Reintegration Core should feel like a playable proof system.

Every sector should ask:

1. What is broken?
2. How does Eli know?
3. Which tool proves or repairs it?
4. What pressure makes the choice matter?
5. What validates the outcome?

If a sector cannot answer those questions, it is not mature enough.

The door is still the proof gate.
The glyph is still evidence.
The relay is still confirmation.
The shower is still recovery.
The tool is still intervention.
Green is still not proof.
