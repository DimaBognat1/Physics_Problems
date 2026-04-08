# 8. Waves

## Given

We need to check which of the following functions can describe a traveling wave by testing the wave equation:

∂²y/∂x² = (1 / v²) ∂²y/∂t²

The functions are:

a) y(x,t) = A cos(kx² − ωt)

b) y(x,t) = A(x − vt)²

c) y(x,t) = A log(x + vt)

---

## Important idea

A standard traveling wave has the form:

y(x,t) = f(x − vt)  or  y(x,t) = f(x + vt)

Any function of the combination (x − vt) or (x + vt) satisfies the wave equation.

So we can first check the structure of each function.

---

## Part (a)

y(x,t) = A cos(kx² − ωt)

### Step 1: Check the argument

The argument is:

kx² − ωt

This is not of the form:

x − vt  or  x + vt

because it contains x², not x.

### Step 2: Conclusion

This function is not a standard traveling wave and in general does not satisfy the wave equation.

---

## Part (b)

y(x,t) = A(x − vt)²

### Step 1: Check the structure

This is clearly a function of:

(x − vt)

So it has the form:

y(x,t) = f(x − vt)

Therefore it should satisfy the wave equation.

### Step 2: Verify by differentiation

First derivative with respect to x:

∂y/∂x = 2A(x − vt)

Second derivative with respect to x:

∂²y/∂x² = 2A

Now derivative with respect to t:

∂y/∂t = 2A(x − vt)(−v) = −2Av(x − vt)

Second derivative with respect to t:

∂²y/∂t² = 2Av²

Now check the wave equation:

(1 / v²) ∂²y/∂t² = (1 / v²)(2Av²) = 2A

This matches:

∂²y/∂x² = 2A

So the wave equation is satisfied.

### Step 3: Conclusion

This function can describe a traveling wave.

---

## Part (c)

y(x,t) = A log(x + vt)

### Step 1: Check the structure

This is a function of:

(x + vt)

So it has the form:

y(x,t) = f(x + vt)

Therefore it should satisfy the wave equation.

### Step 2: Verify by differentiation

First derivative with respect to x:

∂y/∂x = A / (x + vt)

Second derivative with respect to x:

∂²y/∂x² = −A / (x + vt)²

Now derivative with respect to t:

∂y/∂t = Av / (x + vt)

Second derivative with respect to t:

∂²y/∂t² = −Av² / (x + vt)²

Now check:

(1 / v²) ∂²y/∂t² = (1 / v²) [−Av² / (x + vt)²]

= −A / (x + vt)²

This is exactly equal to:

∂²y/∂x² = −A / (x + vt)²

So the wave equation is satisfied.

### Step 3: Conclusion

This function can also describe a traveling wave.

---

## Final Answer

The functions that can describe a traveling wave are:

b) y(x,t) = A(x − vt)²

c) y(x,t) = A log(x + vt)

The function

a) y(x,t) = A cos(kx² − ωt)

does not describe a traveling wave.
