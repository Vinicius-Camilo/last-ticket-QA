# Bug Reports — LAST TICKET

**Test date:** July 8, 2026  
**Testing method:** Exploratory manual testing  
**Game:** [LAST TICKET](https://ray-casting.itch.io/lastticket)  
**Version recorded in the original review:** v1.0.0

These reports summarize issues observed during an exploratory gameplay session. Reproduction steps are included only where supported by the original observations. Issues have not been independently retested in subsequent builds.

## 1. Player Collision and Environmental Geometry

### BUG-001 — Player Can Walk Through Office Tables

**Category:** Collision Detection  
**Observed behavior:** The player could walk through office tables, with the exception of Maya's table.

**Expected behavior:** Solid environmental objects should consistently prevent the player from passing through them unless intentional.

**Reproduction notes:** Attempt to walk into the office tables. The behavior was not consistent across all tables.

### BUG-002 — Player Can Walk Through Environmental Objects

**Category:** Collision Detection  
**Observed behavior:** The player could walk through a plant and a barrel outside the office.

**Expected behavior:** Objects intended to occupy solid space should have appropriate collision boundaries.

### BUG-003 — Crouching Under a Desk Causes Clipping and Unexpected Repositioning

**Category:** Character Movement / Collision  
**Observed behavior:** Crouching under the office desk visually appeared to clip the character through the furniture. Standing up while underneath caused the character to be repositioned above or beside the desk.

**Expected behavior:** Character movement should respect furniture geometry and avoid unintended repositioning.

### BUG-004 — Opening the Gate Can Trap the Player

**Category:** Collision / Level Geometry  
**Observed behavior:** When positioned directly below the gate above the office entrance, opening it caused the player to become stuck. Closing the gate or crouching away allowed the player to move again.

**Expected behavior:** Opening the gate should not trap the player in an unintended state.

## 2. Hiding and Animation

### BUG-005 — Crouch State Persists After Entering a Locker

**Category:** Character State / Gameplay Mechanics  
**Observed behavior:** After crouching to enter a locker, the character remained crouched. The character could still stand up and, in some instances, crouch again.

**Expected behavior:** Character posture and hiding states should transition consistently when entering and leaving a locker.

### BUG-006 — Head Bobbing Animation Continues Inside a Locker

**Category:** Animation  
**Observed behavior:** When entering a locker while moving, the character's head-bobbing animation sometimes continued while the character was inside.

**Expected behavior:** Movement animations should reflect the character's current state and should not continue when inappropriate for the hiding state.

## 3. Object Interaction and Item Handling

### BUG-007 — Object Interactions Unavailable During a Guided Sequence

**Category:** Interaction / Gameplay Progression  
**Observed behavior:** During the sequence in which the NPC "Maya" showed the player around, I was unable to interact with objects. Doors remained interactable.

**Expected behavior:** Interactions should remain available when intended by the current gameplay sequence.

### BUG-008 — Dropped Item Can Fall Outside the Playable Area

**Category:** Item Handling / Level Boundaries  
**Observed behavior:** While inside a locker, the player could drop an object. Looking back into the locker and dropping the object caused it to fall outside the playable area.

**Expected behavior:** Dropped items should remain accessible within the playable environment or follow the intended item-handling rules.

## 4. Input and Controls

### BUG-009 — Pressing T Stops Character Movement

**Category:** Input Handling  
**Observed behavior:** Pressing the T key completely stopped character movement during the session.

**Expected behavior:** Character movement should not be interrupted by an unexplained input.

**Notes:** The cause was not determined. The observation may warrant investigation of input bindings and game state handling.

### OBS-001 — Unexpected Speed Changes When Using Plus and Minus Keys

**Category:** Input Handling  
**Observed behavior:** Pressing the plus and minus keys appeared to change the game's speed.

**Expected behavior:** If these inputs are not intended as player-facing controls, they should not unexpectedly alter gameplay.

**Notes:** The cause was not confirmed.

### OBS-002 — Mouse Sensitivity Remains High at the Minimum Setting

**Category:** Controls / Settings  
**Observed behavior:** Mouse sensitivity remained too high for comfortable control, even when the setting was at its minimum.

**Expected behavior:** The minimum sensitivity setting should provide a meaningfully lower sensitivity level.

## 5. Gameplay Progression

### OBS-003 — Ticket Event Did Not Appear to Progress

**Category:** Gameplay Progression / Event Handling  
**Observed behavior:** During both sessions, the expected "ticket arrival" event did not happen despite waiting for it. The gameplay recording included the waiting period.

**Expected behavior:** The ticket event should occur when the required progression conditions have been met.

**Notes:** The exact trigger conditions and intended waiting duration were not established. The observation does not independently confirm the underlying cause.

## 6. Visual and Text Quality

### OBS-004 — Calendar Contains Noticeable Visual and Text Issues

**Category:** Visual Quality  
**Observed behavior:** The office calendar contained noticeable visual inconsistencies and apparent mistakes.

**Expected behavior:** Environmental assets should meet the intended visual quality standard and avoid distracting inconsistencies.

### OBS-005 — Grammar Issues in Dialogue

**Category:** Text Quality / Localization  
**Observed behavior:** Grammar issues were noticed in several places, particularly in one of the NPC's dialogue concerning the copying of voices.

**Expected behavior:** In-game text should be grammatically correct and consistent with the intended meaning.

## Summary

The session revealed issues across collision detection, hiding mechanics, object interaction, input handling, gameplay progression, and presentation.

The findings were shared with the developer through the original review. No claims are made here regarding the status of these issues in later builds.
