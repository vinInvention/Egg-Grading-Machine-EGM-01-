# Engineering Notebook (Every work session gets a new entry.)

---

## Date

Objective

---

Work Completed

---

Problems Encountered

---

Ideas

---

Decisions Made

---

Next Steps

---

## Phase 2.6 — Chain and Sprocket Selection Study

Engineering Lesson #17

One of the biggest mistakes beginner designers make is this:

"I bought a chain because it looked strong."

Engineers don't ask,

"Is it strong?"

They ask,

"Is it the smallest, lightest, least expensive chain that safely meets the design requirements?"

Oversizing a machine is just as bad as undersizing it.

A heavier chain means:

More inertia
Larger motor
Larger bearings
Higher cost
More maintenance

For EGM-01, our load is actually quite small.

So let's choose the chain scientifically.

## Engineering Calculation

Now that we've selected a #35 chain with a 15-tooth sprocket, we can update our earlier assumptions.

For a #35 chain:

Pitch = 9.525 mm

Pitch circumference:

15×9.525=142.875 mm

Pitch diameter:

D=
π
142.875
​

D≈45.5 mm

We'll use:

Pitch Diameter = 46 mm

Radius:

23 mm

Notice that this slightly changes our torque calculations, but not significantly.

Why 15 Teeth Instead of 12?

This is an important design decision.

12 Teeth 15 Teeth
Smaller diameter Slightly larger diameter
Higher chain wear Lower chain wear
More vibration Smoother operation
More polygon effect Reduced polygon effect
Shorter chain life Longer chain life

The polygon effect is a phenomenon where a chain does not move perfectly smoothly around a small sprocket because it wraps around discrete teeth rather than a perfect circle. Increasing the number of teeth reduces this effect, giving smoother motion—an advantage when transporting fragile eggs.
