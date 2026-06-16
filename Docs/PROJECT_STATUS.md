# Project Status

Last updated: 2026-06-16

## Current Checkpoint

Night Shift Ticket is currently at the end of M2.5. The project has a playable first-person blockout route and is ready for the first minimal PC ticket interaction smoke test.

## Completed Milestones

### M1: Project Foundation

Status: DONE

- Unreal Engine First Person Blueprint project created.
- Git repository set up.
- Basic project documentation added.
- Blueprint-first direction confirmed.
- First phase confirmed as offline, with no live OpenAI/API runtime dependency.

### M2: Basic Movement And Space

Status: DONE

- First-person movement works.
- Player can walk through the current map.
- Current blockout contains:
  - IT office / base room,
  - desk and PC,
  - hallway,
  - meeting room / zasedacka.
- Route IT office -> hallway -> meeting room -> back is playable and tested.

### M2.5: Blockout Readability And Meeting Room Props

Status: DONE

- Basic lighting added.
- Meeting room contains a table and multiple chairs.
- Reusable blockout chair Blueprint created.
- Meeting room contains a projector.
- Meeting room contains a projection screen.
- Hidden-message placeholder prepared on or near the screen for the future camera mechanic.
- Level was tested, committed, and pushed.

## Current Constraints

- Keep development in small verified steps.
- Do not add combat.
- Do not add inventory yet.
- Do not add save/load yet.
- Do not add a full ticket state machine yet.
- Do not add the camera mechanic yet.
- Do not introduce C++.
- Do not add external frameworks or Fab assets.
- Keep Blueprint work beginner-friendly and readable.

## Next Milestone

### M3: First PC Ticket Interaction

Immediate target: M3.1 minimal interaction smoke test.

Expected behavior:

1. Player approaches the PC in the IT office.
2. Player presses E.
3. A simple ticket text appears.
4. Pressing E again or Escape hides the ticket text.

First ticket text:

```text
Ticket #001
Location: Meeting Room
Issue: Projector turns on by itself after midnight.
Instruction: Check the meeting room and report evidence.
```

M3.1 should stay intentionally small. It only needs to prove that the player can interact with the PC and show/hide ticket text in the editor.
