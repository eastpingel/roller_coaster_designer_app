# Prompt Log

## 2026-11-23

- **Asked:** Create `AGENTS.md`, `prompts.md`, and `index.html`; keep a log entry after every request.
- **Changed:** Created the agent instructions, prompt log, and a complete single-page roller coaster designer interface.
- **Worked:** Yes.

## 2026-11-24

- **Asked:** Read the Roller Coaster Designer specification, ask clarifying questions, and build the web app.
- **Changed:** Replaced the interface mock with a draggable control-point track editor, conservation-of-energy speed calculations, vertical g-force plots, failure markers and rollback animation, thrill scoring, a physics popup, local browser saving, and keyboard-accessible controls.
- **Worked:** Yes. The app loads successfully and rendered correctly in the browser at the local server URL.

- **Asked:** Fix the ride animation because the coaster did not move.
- **Changed:** Removed the extra repeated starting spline segment that trapped the car at zero speed, and changed animation stepping to advance by traveled distance while accounting for zero-length sample duplicates.
- **Worked:** Yes. Browser testing confirmed that clicking Ride moves the car downhill and updates its speed readout.

- **Asked:** Make the car move faster and slower based on its displayed speed.
- **Changed:** Mapped physical speed to the sampled curve's full screen-space length instead of its horizontal width, keeping movement distance proportional to the live mph readout.
- **Worked:** Yes. Browser testing confirmed the car advances and its speed and movement both increase as it descends.

- **Asked:** Multiply the car's speed by 2.
- **Changed:** Applied a 2x multiplier to animation distance per frame while leaving the physics speed readout unchanged.
- **Worked:** Yes. The animation step now uses exactly twice the computed average speed.

- **Asked:** Multiply the car's speed by 2 again.
- **Changed:** Doubled the animation multiplier from 2x to 4x without changing the displayed physics speed.
- **Worked:** Yes. The animation now advances at four times the unscaled calculated rate.
