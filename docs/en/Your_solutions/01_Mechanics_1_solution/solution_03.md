# Section 1 — Path Intersection

We are given:

A(t) = (2 + t, 8 − 3t)  
B(t) = (2t − 1, 2t + 2)  

---

## Solution

### Step 1: Check if paths intersect

Set coordinates equal:

2 + t = 2t − 1  
8 − 3t = 2t + 2  

---

### Step 2: Solve first equation

2 + t = 2t − 1  

2 + 1 = 2t − t  

t = 3  

---

### Step 3: Check second equation

8 − 3(3) = 2(3) + 2  

8 − 9 = 6 + 2  

−1 ≠ 8 ❌  

---

### Step 4: Conclusion

The paths do not intersect.

---

### Step 5: Minimum distance

Distance between points:

d(t) = √[(x₁ − x₂)² + (y₁ − y₂)²]

x₁ − x₂ = (2 + t) − (2t − 1) = 3 − t  
y₁ − y₂ = (8 − 3t) − (2t + 2) = 6 − 5t  

d²(t) = (3 − t)² + (6 − 5t)²  

---

### Step 6: Minimize distance

d²(t) = (3 − t)² + (6 − 5t)²  

= (t − 3)² + (5t − 6)²  

Derivative:

d/dt = 2(t − 3) + 10(5t − 6)  

= 2t − 6 + 50t − 60  

= 52t − 66  

Set to zero:

52t = 66  

t = 66 / 52 ≈ 1.27  

---

## Final Answer

The paths do not intersect.  

Minimum distance occurs at:

t ≈ 1.27  
