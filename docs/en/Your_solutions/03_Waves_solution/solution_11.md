# 11. Animation: Two-Slit Interference

## Problem

We need to create an HTML animation simulating Young's double-slit experiment.

Two slits act as coherent point sources.  
The total displacement is the sum of two partial waves:

u(r, t) = u₁(r, t) + u₂(r, t)

where each source generates a circular wave.

The user should be able to change:

- the distance between the slits d
- the wavelength λ

The animation should show the interference pattern in real time.

---

## Idea of the solution

Two fixed sources are placed on the screen.

For every point of the observation region, we calculate:

u₁(r,t) = A / |r − r₁| sin(k|r − r₁| − ωt)

u₂(r,t) = A / |r − r₂| sin(k|r − r₂| − ωt)

Then the total displacement is:

u(r,t) = u₁(r,t) + u₂(r,t)

The color on the screen represents the resulting displacement, which makes constructive and destructive interference visible.

---

## Features of the animation

- slider for slit distance d
- slider for wavelength λ
- real-time interference pattern
- visible slit positions

---

## Physical interpretation

Bright regions correspond to constructive interference.  
Dark regions correspond to destructive interference.  
Changing the slit distance and wavelength changes the interference pattern.
