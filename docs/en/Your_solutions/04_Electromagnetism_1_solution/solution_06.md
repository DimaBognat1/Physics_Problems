# 6. Field at a Point from a System of Charges

## Given

Two point charges are placed on the x-axis:

- charge \(+q\) at point \((-a, 0)\)
- charge \(+2q\) at point \((a, 0)\)

We need to:

1. determine the electric field vector \(\vec E(0,y)\), \(\vec E(x,0)\), and in general \(\vec E(x,y)\)
2. determine the condition for which \(E_x = 0\), \(E_y = 0\), and \(\vec E = 0\)
3. calculate the field for \(a = 0.2\text{ m}\), \(y = 0.3\text{ m}\), \(q = 2\,\mu\text{C}\)
4. investigate the limit \(y \gg a\)

---

## Step 1: General formula for the electric field of a point charge

For a point charge \(Q\) located at position \(\vec r_0\), the electric field at point \(\vec r\) is:

\[
\vec E(\vec r) = kQ \frac{\vec r - \vec r_0}{|\vec r - \vec r_0|^3}
\]

where:

- \(k = 9 \times 10^9 \text{ N·m}^2/\text{C}^2\)

---

## Step 2: Write the contribution from each charge

Let the observation point be:

\[
\vec r = (x,y)
\]

### Field from charge \(+q\) at \((-a,0)\)

The displacement vector from this charge to the point is:

\[
\vec r_1 = (x+a,\, y)
\]

Its distance is:

\[
r_1 = \sqrt{(x+a)^2 + y^2}
\]

So the field is:

\[
\vec E_1 = kq \frac{(x+a,\, y)}{\left[(x+a)^2 + y^2\right]^{3/2}}
\]

---

### Field from charge \(+2q\) at \((a,0)\)

The displacement vector is:

\[
\vec r_2 = (x-a,\, y)
\]

Its distance is:

\[
r_2 = \sqrt{(x-a)^2 + y^2}
\]

So the field is:

\[
\vec E_2 = k(2q) \frac{(x-a,\, y)}{\left[(x-a)^2 + y^2\right]^{3/2}}
\]

---

## Step 3: General electric field \(\vec E(x,y)\)

Add both contributions:

\[
\vec E(x,y) = \vec E_1 + \vec E_2
\]

Therefore:

\[
\vec E(x,y)
=
kq \frac{(x+a,\, y)}{\left[(x+a)^2 + y^2\right]^{3/2}}
+
2kq \frac{(x-a,\, y)}{\left[(x-a)^2 + y^2\right]^{3/2}}
\]

So the components are:

\[
E_x
=
kq \frac{x+a}{\left[(x+a)^2 + y^2\right]^{3/2}}
+
2kq \frac{x-a}{\left[(x-a)^2 + y^2\right]^{3/2}}
\]

\[
E_y
=
kq \frac{y}{\left[(x+a)^2 + y^2\right]^{3/2}}
+
2kq \frac{y}{\left[(x-a)^2 + y^2\right]^{3/2}}
\]

---

## Step 4: Field on the y-axis, \(\vec E(0,y)\)

Set \(x=0\).

Then:

\[
E_x(0,y)
=
kq \frac{a}{(a^2+y^2)^{3/2}}
+
2kq \frac{-a}{(a^2+y^2)^{3/2}}
\]

\[
E_x(0,y)
=
kq \frac{a-2a}{(a^2+y^2)^{3/2}}
=
-kq \frac{a}{(a^2+y^2)^{3/2}}
\]

Now for the y-component:

\[
E_y(0,y)
=
kq \frac{y}{(a^2+y^2)^{3/2}}
+
2kq \frac{y}{(a^2+y^2)^{3/2}}
\]

\[
E_y(0,y)
=
3kq \frac{y}{(a^2+y^2)^{3/2}}
\]

So:

\[
\vec E(0,y)
=
\left(
-kq \frac{a}{(a^2+y^2)^{3/2}},
\;
3kq \frac{y}{(a^2+y^2)^{3/2}}
\right)
\]

---

## Step 5: Field on the x-axis, \(\vec E(x,0)\)

Set \(y=0\).

Then the field has only x-component, because all charges and the point lie on the x-axis.

So:

\[
E_y(x,0)=0
\]

And:

\[
E_x(x,0)
=
kq \frac{x+a}{|x+a|^3}
+
2kq \frac{x-a}{|x-a|^3}
\]

Therefore:

\[
\vec E(x,0)
=
\left(
kq \frac{x+a}{|x+a|^3}
+
2kq \frac{x-a}{|x-a|^3},
\;
0
\right)
\]

---

## Step 6: Conditions for \(E_x=0\), \(E_y=0\), and \(\vec E=0\)

### Condition for \(E_y=0\)

From the general formula:

\[
E_y
=
kq \frac{y}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq \frac{y}{\left[(x-a)^2+y^2\right]^{3/2}}
\]

Factor out \(y\):

\[
E_y = y \left[
kq \frac{1}{\left[(x+a)^2+y^2\right]^{3/2}}
+
2kq \frac{1}{\left[(x-a)^2+y^2\right]^{3/2}}
\right]
\]

The bracket is always positive, so the only way \(E_y=0\) is:

\[
y=0
\]

So the zero of the y-component occurs only on the x-axis.

---

### Condition for \(E_x=0\) on the x-axis

Now use \(y=0\), so:

\[
E_x(x,0)
=
kq \frac{x+a}{|x+a|^3}
+
2kq \frac{x-a}{|x-a|^3}
\]

The point where total field can vanish must be between the charges, because outside the interval both contributions point in the same direction.

So assume:

\[
-a < x < a
\]

Then:

- \(x+a > 0\)
- \(x-a < 0\)

Thus:

\[
\frac{x+a}{|x+a|^3} = \frac{1}{(x+a)^2}
\]

\[
\frac{x-a}{|x-a|^3} = -\frac{1}{(a-x)^2}
\]

So:

\[
E_x = kq\frac{1}{(x+a)^2} - 2kq\frac{1}{(a-x)^2}
\]

Set \(E_x=0\):

\[
\frac{1}{(x+a)^2} = \frac{2}{(a-x)^2}
\]

Cross-multiply:

\[
(a-x)^2 = 2(x+a)^2
\]

Take square root:

\[
a-x = \sqrt{2}(x+a)
\]

Solve:

\[
a-x = \sqrt2 x + \sqrt2 a
\]

\[
a-\sqrt2 a = x + \sqrt2 x
\]

\[
a(1-\sqrt2) = x(1+\sqrt2)
\]

\[
x = a \frac{1-\sqrt2}{1+\sqrt2}
\]

Multiply numerator and denominator by \(1-\sqrt2\):

\[
x = a(1-\sqrt2)^2 / (1-2)
\]

\[
x = -a(1-\sqrt2)^2
\]

Numerically:

\[
x \approx -0.1716\,a
\]

So the zero-field point is on the x-axis, between the charges, closer to the smaller charge \(+q\).

---

### Condition for \(\vec E=0\)

For the total field to be zero, both components must vanish:

- \(E_y=0 \Rightarrow y=0\)
- \(E_x=0\) gives the point above

Therefore, the only zero-field point is:

\[
y=0,\qquad
x = a \frac{1-\sqrt2}{1+\sqrt2}
\]

---

## Step 7: Numerical calculation for \(a=0.2\text{ m}\), \(y=0.3\text{ m}\), \(q=2\,\mu\text{C}\)

We are asked for the field at \((0,y)\), so use the formula from Step 4.

Given:

\[
a = 0.2
\]

\[
y = 0.3
\]

\[
q = 2\times 10^{-6}\text{ C}
\]

\[
k = 9\times 10^9
\]

First compute:

\[
a^2+y^2 = 0.2^2 + 0.3^2 = 0.04 + 0.09 = 0.13
\]

\[
(a^2+y^2)^{3/2} = 0.13^{3/2}
\]

\[
\sqrt{0.13} \approx 0.3606
\]

\[
0.13^{3/2} = 0.13 \times 0.3606 \approx 0.0469
\]

Now:

\[
kq = 9\times 10^9 \times 2\times 10^{-6}
= 18\times 10^3 = 18000
\]

### x-component

\[
E_x = -kq\frac{a}{(a^2+y^2)^{3/2}}
\]

\[
E_x = -18000 \cdot \frac{0.2}{0.0469}
\]

\[
E_x \approx -7.68 \times 10^4 \text{ N/C}
\]

### y-component

\[
E_y = 3kq\frac{y}{(a^2+y^2)^{3/2}}
\]

\[
E_y = 3 \cdot 18000 \cdot \frac{0.3}{0.0469}
\]

\[
E_y \approx 3.45 \times 10^5 \text{ N/C}
\]

So:

\[
\vec E(0,0.3)
\approx
(-7.68\times 10^4,\; 3.45\times 10^5)\text{ N/C}
\]

---

## Step 8: Limit \(y \gg a\)

From:

\[
\vec E(0,y)
=
\left(
-kq \frac{a}{(a^2+y^2)^{3/2}},
\;
3kq \frac{y}{(a^2+y^2)^{3/2}}
\right)
\]

If \(y \gg a\), then:

\[
a^2+y^2 \approx y^2
\]

and therefore:

\[
(a^2+y^2)^{3/2} \approx y^3
\]

So:

\[
E_x \approx -kq \frac{a}{y^3}
\]

\[
E_y \approx 3kq \frac{1}{y^2}
\]

This means:

- the x-component becomes very small, because it falls as \(1/y^3\)
- the y-component dominates, because it falls as \(1/y^2\)

So far away from the charges, the system behaves approximately like a single charge of total value:

\[
q_{total} = q + 2q = 3q
\]

located near the origin.

---

## Final Answer

### General field:

\[
\vec E(x,y)
=
kq \frac{(x+a,\, y)}{\left[(x+a)^2 + y^2\right]^{3/2}}
+
2kq \frac{(x-a,\, y)}{\left[(x-a)^2 + y^2\right]^{3/2}}
\]

### On the y-axis:

\[
\vec E(0,y)
=
\left(
-kq \frac{a}{(a^2+y^2)^{3/2}},
\;
3kq \frac{y}{(a^2+y^2)^{3/2}}
\right)
\]

### On the x-axis:

\[
\vec E(x,0)
=
\left(
kq \frac{x+a}{|x+a|^3}
+
2kq \frac{x-a}{|x-a|^3},
\;
0
\right)
\]

### Zero-field point:

\[
y=0,\qquad
x = a \frac{1-\sqrt2}{1+\sqrt2}
\]

### For \(a=0.2\text{ m}, y=0.3\text{ m}, q=2\,\mu\text{C}\):

\[
\vec E(0,0.3)
\approx
(-7.68\times 10^4,\; 3.45\times 10^5)\text{ N/C}
\]

### For \(y\gg a\):

\[
E_x \approx -kq \frac{a}{y^3},\qquad
E_y \approx 3kq \frac{1}{y^2}
\]

So at large distances the system behaves approximately like a single charge \(3q\).
