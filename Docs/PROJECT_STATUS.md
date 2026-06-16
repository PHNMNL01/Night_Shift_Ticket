# Project Status

Last updated: 2026-06-16

## Current Checkpoint

Night Shift Ticket is currently at the end of M3.1. The project has a playable first-person blockout route and a tested first PC ticket interaction in the IT office.

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

### M3.1: First PC Ticket Interaction

Status: DONE

- `WBP_TicketText` created as a simple screen-space UI ticket widget.
- `BP_PC_TicketInteractable` created for the PC interaction logic.
- Interaction collision added near the PC as `InteractZone`.
- BeginOverlap detects the player and enables local PC input.
- EndOverlap closes the ticket and disables local PC input.
- The ticket widget reference is created on BeginPlay.
- Pressing E while inside the interaction zone opens the ticket.
- Pressing E again closes the ticket.
- Pressing E again reopens the ticket.
- Walking away from the PC closes the ticket automatically.
- Pressing E outside the interaction zone does nothing.
- Escape/Q close behavior was discussed as optional because Escape can stop PIE in the editor; the tested core behavior is E toggle plus EndOverlap close.

## Current Constraints

- Keep development in small verified steps.
- Do not add combat.
- Do not add inventory yet.
- Do not add save/load yet.
- Do not add a full ticket manager or full ticket state machine yet.
- Do not add the camera mechanic yet.
- Do not introduce C++.
- Do not add external frameworks or Fab assets.
- Keep Blueprint work beginner-friendly and readable.

## Next Milestone

### M3.2: Small Ticket Interaction Polish

Recommended next target: keep M3.2 intentionally small and local to the current PC interaction.

Suggested options:

- Replace the debug "Press E" feedback with a simple on-screen interaction prompt.
- Or add a minimal local ticket state such as New/Active/Viewed inside `BP_PC_TicketInteractable`.

Do not create a full ticket manager yet.

Current tested gameplay behavior:

1. Player walks near the PC in the IT office and sees/debugs "Press E".
2. Player presses E inside the interaction zone.
3. A simple ticket widget appears.
4. Pressing E again closes the ticket.
5. Pressing E again reopens the ticket.
6. Walking away from the PC closes the ticket automatically.
7. Pressing E outside the interaction zone does nothing.

Current first ticket text:

```text
Ticket #001
Location: Meeting Room
Issue: Projector turns on by itself after midnight.
Instruction: Check the meeting room and report evidence.
```
