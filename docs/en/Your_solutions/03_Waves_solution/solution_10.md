# 10. Animation: Wave Sources

## Problem

We need to create an HTML animation in which point sources generate waves described by

u(r, t) = A / |r − r₀|^α * sin(k|r − r₀| − ωt)

where:
- r₀ is the position of a source,
- α is a damping parameter in the range [0, 2].

The animation should show the superposition of waves from all placed sources.

---

## Idea of the solution

The program represents the screen as a 2D grid.

For every grid point, the total displacement is calculated as the sum of contributions from all sources:

u_total = Σ u_i(r, t)

Each source contributes a wave of the form:

u_i(r, t) = A / d_i^α * sin(k d_i − ωt)

where d_i is the distance from the grid point to the source.

The animation updates in time, so the phase changes continuously and the wave pattern moves.

---

## Features of the animation

- click on the canvas to add wave sources,
- show superposition of all waves,
- adjustable damping parameter α,
- adjustable wavelength and frequency,
- clear visualization of interference.

---

## Physical interpretation

Each source emits a circular wave.  
The total pattern is the result of interference between all waves.  
When α increases, the amplitude decreases faster with distance.
