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

## Phase 2.7 — Shaft and Bearing Design Study

Engineering Lesson #18

Many beginners think:

"The shaft just holds the sprocket."

A mechanical engineer thinks:

The shaft transmits torque, supports rotating components, resists bending, maintains alignment, and interfaces with bearings and power transmission elements.

The shaft is much more than a rod.

Step 1 — Functions of the Shaft

Our shaft must:

Support two sprockets.
Transmit motor torque.
Maintain alignment between the chains.
Support the chain tension.
Rotate smoothly inside bearings.
Be easy to manufacture.
Resist bending and twisting.
Step 2 — Candidate Shaft Diameters

Let's compare three common sizes.

Diameter Advantages Disadvantages
8 mm Cheap, lightweight May bend if overloaded, fewer standard sprockets available
10 mm Good balance of strength and weight Slightly heavier than 8 mm
12 mm Very rigid Unnecessary for our relatively light machine
Engineering Analysis

Recall our earlier design:

Moving mass ≈ 2.5 kg
Design torque ≈ 0.4 N·m
Low conveyor speed
Horizontal conveyor
Short shaft span (less than 500 mm)

This is not a heavy-duty conveyor.

An 8 mm shaft could probably work, but it leaves little margin for future upgrades or accidental overload.

A 12 mm shaft is unnecessarily heavy and increases bearing and coupling costs.

A 10 mm shaft provides a good balance.

Preliminary Engineering Decision

Use a 10 mm steel shaft

Step 3 — Shaft Material

Candidate materials:

Mild Steel (AISI 1018 / Equivalent)

Advantages:

Inexpensive
Easy to machine
Easy to weld
Widely available

Disadvantages:

Can rust
Stainless Steel

Advantages:

Corrosion resistant
Food industry friendly

Disadvantages:

Expensive
Harder to machine
Aluminum

Advantages:

Lightweight

Disadvantages:

Lower stiffness
Lower wear resistance
Final Material Decision

For Version 1:

10 mm Mild Steel Shaft

Reason:

Affordable, easy to machine, and readily available locally.

Step 4 — Bearing Selection

Now we select bearings.

Candidate options:

Bearing Suitable? Notes
608 Skate Bearing ❌ Designed for light radial loads, awkward to mount on machinery
6000 Series ✅ General-purpose deep groove bearing
6200 Series ✅ Higher load capacity
Pillow Block Bearing ⭐⭐⭐⭐⭐ Easy mounting, excellent shaft alignment
Bronze Bushings ⚠️ Higher friction, more wear
Why Pillow Block Bearings?

A pillow block combines:

Bearing
Housing
Mounting holes
Shaft support

Instead of machining a precise bearing pocket, you simply bolt the bearing assembly to the frame.

Advantages:

Easy installation
Easy replacement
Better alignment
Ideal for prototype machines
Recommended Bearing
UCP201 Pillow Block

Specifications:

Shaft diameter: 12 mm

Since we selected a 10 mm shaft, a better match is:

UCP200 Series for 10 mm shaft (or equivalent locally available unit)

When purchasing, verify the bore size matches your shaft. Many suppliers also offer metric pillow blocks specifically for 10 mm shafts.

Step 5 — Shaft Layout
Motor Coupling

      │

      ▼

Bearing

      │

      ▼

Sprocket

      │

      ▼

Spacer

      │

      ▼

Second Sprocket

      │

      ▼

Bearing

Notice something?

The bearings are outside the sprockets.

Why?

Because the sprockets should sit between the bearings.

This reduces shaft bending.

Step 6 — Sprocket Mounting

How should we attach the sprocket?

Options:

Set Screw

Advantages:

Cheap
Easy

Disadvantages:

Can loosen over time
Keyway

Advantages:

Strong
Reliable

Disadvantages:

Requires machining
D-shaped Shaft

Advantages:

Easy
Good torque transmission

Disadvantages:

Less common
Engineering Decision

For Version 1:

Use set-screw sprockets with thread-locking compound.

This keeps manufacturing simple.

Future versions can move to keyed shafts if needed.

Step 7 — Chain Tensioning

A chain must never be installed perfectly tight.

It needs a small amount of slack.

Recommended methods:

Adjustable motor mount
Sliding bearing mount
Idler sprocket

For EGM-01:

Adjustable bearing slots

This allows fine adjustment after assembly.
