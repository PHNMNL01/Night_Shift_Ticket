# Night Shift Ticket

## Short Description

Night Shift Ticket is a short first-person atmospheric horror game built in Unreal Engine. The player is a night-shift IT worker in an office building, handling seemingly ordinary incidents through a ticketing system. Over time, it becomes clear that the problems are not just technical. They are connected to a hidden layer of reality that can only be revealed through a camera.

The first target is a small 5 to 10 minute playable demo with no combat.

## Main Vision

The game is built around a work routine that slowly collapses into horror. The ticketing system gives the player clear tasks, while the environment, sound design, and visual changes suggest that the building is responding to their progress.

The horror should not feel random. Every frightening moment should have a signal, a reason, or a rule behind it. The player should feel like they have understood something, even if they cannot fully trust that understanding yet.

The main mechanic is the camera. It does not simply show ghosts. It reveals a more truthful version of a place: messages, traces, silhouettes, objects, or changes that are invisible in normal view. Photographing the correct discovery advances the ticket, changes the state of the environment, or triggers a short horror event.

## Core Gameplay Loop

1. The player starts in the IT office.
2. A new ticket appears on the PC.
3. The player goes to the assigned room.
4. In normal view, the issue is invisible or appears mundane.
5. Through the camera, the hidden layer of reality is revealed.
6. The player takes a photo as evidence.
7. The player returns to the PC.
8. The ticket is updated or closed.
9. The environment changes slightly after each ticket.

## First Vertical Slice

The first vertical slice should prove that the core combination of tickets, movement through the building, camera-based discovery, and atmospheric change works as a playable foundation.

The first slice includes:

- one IT office as the base with a PC and ticketing system,
- one hallway,
- one meeting room,
- one ticket,
- one camera-only discovery,
- one photo used as evidence,
- one ticket update after returning to the PC,
- one short horror event tied to completing the ticket.

## First Version Constraints

- No combat.
- No inventory system in the first phase.
- No save/load system in the first phase.
- No live OpenAI API runtime in the first phase.
- The game should run offline in the first phase.
- AI may help with writing, tickets, documentation, and Blueprint logic design, but it should not be a runtime dependency.
- The map scope is limited to a few small spaces.
- The first version should not try to cover the full game scope. It should only validate the core feeling and loop.

## Milestone Plan

### M1: Project Foundation

- create a clean Unreal Engine project,
- set up Git and the basic documentation structure,
- define the vision, constraints, and first vertical slice,
- confirm the Blueprint-first approach.

### M2: Basic Movement And Space

- create simple first-person movement,
- build a placeholder level: IT office, hallway, meeting room,
- set up basic lighting and early atmosphere,
- verify that the map is walkable.

### M3: Ticket Loop

- create a simple PC/ticket interaction flow,
- display one ticket,
- allow the player to accept or track the task,
- return to the PC and update the ticket.

### M4: Camera Mechanic

- add a usable camera or camera-view mode,
- show an object or trace that is visible only through the camera,
- detect when the correct discovery is photographed,
- connect the discovery to the ticket state.

### M5: First Horror Event

- change the environment after the ticket is completed,
- add one short atmospheric event,
- test pacing, readability, and tension,
- keep the event rule-based rather than random.

### M6: Vertical Slice Polish

- polish the flow from the start to the end of the demo,
- add basic sounds, text, and feedback,
- remove blockers in playability,
- prepare the first shareable build or walkthrough video.

## Development Rule

Development happens in small verified steps. Each step should be self-contained, understandable, and testable directly in the editor or in a playable build once completed.

Do not add large systems too early. First, verify that the main camera + ticket loop feels good. Only after that should the map, atmosphere, story, and more complex systems be expanded.

## Technical Direction

The project is currently Blueprint-first. The first prototypes and gameplay systems will be built in Blueprints so development stays fast, readable, and useful for learning Unreal Engine.

C++ will be introduced later only if it is genuinely needed for performance, more complex architecture, or a system that becomes unnecessarily awkward in Blueprints.
