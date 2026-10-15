# Dunes Tower Defense

A physical, sandbox tower-defense game built from scratch at **Build18 2026**
(Carnegie Mellon ECE's 168-hour hardware hackathon). Players shape real sand in a
sandbox; a depth camera turns that terrain into the game map in real time, and
physical tower pieces placed in the sand become in-game towers that defend
against waves of enemies pathing over the changing landscape.

**Build18 Officer's Choice Award winner** (one of six awards across 100+ teams).

## What it does

- **Sand becomes the map.** A depth camera reconstructs the sandbox surface as a
  live heightmap; a topographic view is projected back onto the sand, so the
  physical terrain and the game world stay in sync as players reshape it.
- **Real pieces become towers.** Computer vision (OpenCV) detects physical tower
  pieces placed in the sandbox and registers them as towers in game state.
- **Enemies adapt to the terrain.** Pathfinding routes enemies over the current
  elevation and tower layout, recomputing as the sand and towers change.
- **From-scratch engine.** No game engine: the rendering, game loop, input, and
  audio were all built directly.

## Tech

- **C++** core game and engine
- **OpenGL** for rendering; **SDL / SFML** for the game loop, input, and audio
- **OpenCV** for tower-piece detection and depth-camera processing
- **Depth camera** for real-time sand-surface heightmap reconstruction
- Projector-based topographic overlay onto the physical sandbox

## About this repository

This is my personal, correctly-attributed copy of a **Build18 team project**. It
was built collaboratively over the hackathon; commit authorship in this fork is
set to me by agreement among the team so each of us can showcase the work under
our own account.

My work centered on the computer-vision and terrain pipeline: depth-camera
heightmap reconstruction, OpenCV tower-piece detection, and enemy pathfinding
over the dynamic terrain.

## Media

Demo photos and video from the sandbox build are added under `media/` (in
progress).
