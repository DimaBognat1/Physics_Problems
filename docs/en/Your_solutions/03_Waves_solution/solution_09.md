# 9. Damped Oscillator

We are given the differential equation of a damped harmonic oscillator:

m d²x/dt² + b dx/dt + kx = 0

We need to:

1. write the general solution,
2. classify the three cases,
3. present the numerical form used in RK4,
4. explain the effect of parameter b,
5. describe the graph of x(t),
6. describe the phase portrait.

---

## Step 1: Rewrite the equation

Divide the whole equation by m:

d²x/dt² + (b/m) dx/dt + (k/m)x = 0

This is a linear second-order differential equation with constant coefficients.

---

## Step 2: Characteristic equation

Assume a solution of the form:

x(t) = e^(rt)

Then:

dx/dt = re^(rt)
d²x/dt² = r²e^(rt)

Substitute into the equation:

m r² e^(rt) + b r e^(rt) + k e^(rt) = 0

Since e^(rt) ≠ 0, we get:

m r² + b r + k = 0

This is the characteristic equation.

---

## Step 3: Solve the characteristic equation

The roots are:

r = [ -b ± √(b² - 4mk) ] / 2m

The behavior of the system depends on the discriminant:

Δ = b² - 4mk

---

## Step 4: Classification of cases

### Case 1: Underdamped motion

If:

b² < 4mk

then the roots are complex:

r = -b/(2m) ± iω_d

where:

ω_d = √(4mk - b²) / 2m

So the solution is:

x(t) = e^(-bt/2m) [ C₁ cos(ω_d t) + C₂ sin(ω_d t) ]

### Interpretation

The system oscillates, but the amplitude decreases with time because of damping.

---

### Case 2: Critically damped motion

If:

b² = 4mk

then the two roots are equal:

r = -b / 2m

The solution is:

x(t) = (C₁ + C₂ t)e^(-bt/2m)

### Interpretation

The system returns to equilibrium as fast as possible without oscillating.

---

### Case 3: Overdamped motion

If:

b² > 4mk

then the roots are two different real numbers:

r₁ = [ -b + √(b² - 4mk) ] / 2m
r₂ = [ -b - √(b² - 4mk) ] / 2m

The solution is:

x(t) = C₁ e^(r₁ t) + C₂ e^(r₂ t)

### Interpretation

The system returns to equilibrium without oscillating, but more slowly than in the critically damped case.

---

## Step 5: Numerical form for RK4

To solve the equation numerically, we rewrite it as a system of first-order equations.

Let:

x₁ = x
x₂ = dx/dt = v

Then:

dx₁/dt = x₂

and from the original equation:

m d²x/dt² + b dx/dt + kx = 0

we get:

dx₂/dt = -(b/m)x₂ - (k/m)x₁

So the RK4 system is:

dx/dt = v
dv/dt = -(b/m)v - (k/m)x

This is the form used in numerical simulation.

---

## Step 6: Effect of parameter b

The parameter b controls the damping strength.

- If b is small, the system is underdamped and oscillates for a long time.
- If b increases, the oscillations decay faster.
- At the critical value:

b_crit = 2√(mk)

the system becomes critically damped.
- If b is larger than this value, the system becomes overdamped.

So increasing b reduces oscillations and makes the motion more strongly damped.

---

## Step 7: Graph of x(t)

### Underdamped case

The graph of x(t) is an oscillating curve with decreasing amplitude.

### Critically damped case

The graph returns to zero quickly without oscillation.

### Overdamped case

The graph also returns to zero without oscillation, but slower than the critically damped case.

---

## Step 8: Phase portrait

The phase portrait is drawn in the plane (x, v).

### Underdamped case

The trajectory spirals toward the origin.

### Critically damped case

The trajectory approaches the origin without spiraling.

### Overdamped case

The trajectory also approaches the origin without spiraling, but more slowly.

In every case, the origin (0,0) is the equilibrium point.

---

## Final Answer

The damped harmonic oscillator

m d²x/dt² + b dx/dt + kx = 0

has three cases depending on the discriminant b² - 4mk:

### Underdamped:
b² < 4mk

x(t) = e^(-bt/2m) [ C₁ cos(ω_d t) + C₂ sin(ω_d t) ]

### Critically damped:
b² = 4mk

x(t) = (C₁ + C₂ t)e^(-bt/2m)

### Overdamped:
b² > 4mk

x(t) = C₁ e^(r₁ t) + C₂ e^(r₂ t)

For RK4, use the system:

dx/dt = v
dv/dt = -(b/m)v - (k/m)x

Increasing b increases damping and changes the motion from oscillatory to non-oscillatory.
