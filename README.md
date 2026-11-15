# LOST-IN-SPACE

**Every explorer has a story. Even the ones we left behind.**

An interactive, game-like website that tells the stories of human-made machines left across the solar system. Built for the NASA Space Apps Challenge 2026, Bangalore.

> Independent work. Not affiliated with or endorsed by NASA.

## Overview

Since the 1960s we have left rovers, landers and probes across the solar system. Their stories sit in technical archives that young learners rarely read. LOST-IN-SPACE turns 15 of them into a playable journey. Fly through a 3D solar system, pick a world, find a machine, scan it, and live its mission in five animated chapters.

It answers one question: **what happens to the explorers we leave behind?**

**Audience:** learners aged 10 and up, and their teachers.

## Features

- **3D solar system:** Sun, eight planets, Earth's Moon, an asteroid belt and a Deep Space marker. Drag to orbit, scroll to zoom, tap a world to select it.
- **Artifact scan:** an animated scan leads to an "Artifact identified" card with name, mission, destination, launch, status and location type.
- **Five-chapter stories:** The Call, The Journey, The Mission, The Discoveries and The Silence, each with a moving diagram and a link to its NASA source.
- **Discovery tracking:** finishing a story unlocks the artifact. Progress is saved in the browser.
- **Database and timeline:** search and filter all artifacts, and see how each generation of missions enabled the next.
- **"Hear its voice":** a short first-person line for each artifact, always labelled as imagination, never as a real transmission.

## The Archive (15 records)

| Destination | Artifacts |
|---|---|
| Moon | Apollo Lunar Modules, Lunar Roving Vehicles, ALSEP Science Stations, Surveyor Landers |
| Mars | Sojourner and Mars Pathfinder, Spirit, Opportunity, Viking 1 and 2, Phoenix, InSight, Ingenuity |
| Asteroids | Dawn (orbiting Ceres), NEAR Shoemaker (Eros) |
| Deep Space | Pioneer 10 and 11, Kepler Space Telescope |

## Scientific Accuracy

- Every artifact is labelled as a confirmed surface, approximate surface, orbital or deep-space location.
- Status and location are kept separate. "Communication lost" describes the machine, not where it is.
- No coordinates are shown rather than inventing them.
- Spirit and Opportunity, and Phoenix and InSight, have separate records because their histories differ.
- The scan is a storytelling interface, not a real scan of the hardware.
- The solar system is not to scale. Planet textures are generated in code, not NASA imagery.

## Run It

The project is one self-contained HTML file. There is no server, no build step and no API keys.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.

An internet connection is needed only to load Three.js from cdnjs.

**Live demo:** [add public link]

## Controls

| Action | Control |
|---|---|
| Rotate view | Drag |
| Zoom | Scroll (desktop) |
| Select a world | Click or tap the planet or its label |
| Jump to a destination | Side list |
| Close any panel | Escape |

Top menu: Explore, Artifacts, Timeline, Discoveries, About.

## Built With

- HTML, CSS and JavaScript
- [Three.js](https://threejs.org/) r128, loaded from cdnjs
- Canvas noise to generate planet textures, so no image files are needed
- Browser `localStorage` for saved progress (key `lis`, with a reset button)

**Accessibility:** keyboard-reachable controls, visible focus outlines, a reduced-motion setting, a mobile layout, and a fallback to lists and stories if WebGL is unavailable.

## NASA Data and References

Mission records were drawn from public NASA pages:

- NASA NSSDCA: https://nssdc.gsfc.nasa.gov
- NASA Science: https://science.nasa.gov

Each artifact links to its NASA source. Mission imagery credit: NASA/JPL where applicable.

## Use of AI

AI tools assisted with code and text development. No AI-generated images or videos are used, and no NASA logos or branding appear in the project.

## Known Limits

- Planet textures are generated, not NASA imagery.
- Not yet built: walkable Moon and Mars scenes, quizzes, achievement badges and sound.

## Team

- Rishika Sharma (Lead)
- Krrish Raj Kannojia
- Siddhi Kapoor
- Pranav Jaiswal
