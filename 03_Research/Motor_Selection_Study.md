Drive System Engineering Calculations
Engineering Lesson #16

A motor is never selected first.

Many beginners say:

"I'm going to use a NEMA 17."

or

"I'll use a JGY370."

Professional engineers ask:

"How much torque does the machine require?"

Only then do they select the motor.

That's exactly what we're going to do.

Step 1 — Estimate the Moving Mass

Let's estimate everything that moves with the conveyor.

Component Estimated Mass
6 Egg carriers 0.60 kg
6 Eggs (maximum 80 g each) 0.48 kg
Two chains 0.70 kg
Mounting brackets 0.20 kg
Miscellaneous fasteners 0.10 kg
Total Moving Mass 2.08 kg

We'll round this up for safety.

Design moving mass = 2.5 kg

We intentionally design for more than expected.

Step 2 — Conveyor Speed

From the previous calculations:

One movement advances 90 mm
One grading cycle takes 5 seconds

Therefore:

Distance per second:

v=
5
0.09
​

=0.018m/s

Conveyor speed = 0.018 m/s

This is intentionally slow to minimize vibration and improve weighing accuracy.

Step 3 — Sprocket Size

We now choose a preliminary sprocket.

Let's assume:

12 teeth
Chain pitch = 12.7 mm (ANSI #40 chain)

Pitch circumference:

12×12.7=152.4mm

Pitch diameter:

D=
π
152.4
​

≈48.5mm

We'll use:

Pitch Diameter = 50 mm

Radius:

r=25mm=0.025m
Step 4 — Required Shaft RPM

Circumference:

C=πD
C=3.142×0.05=0.157m

Every revolution moves:

157 mm

We need:

90 mm every 5 seconds.

Therefore,

Required RPM:

RPM=
0.157
0.018×60
​

RPM≈6.9

Round it:

Required shaft speed ≈ 7 RPM

Notice how slow that is.

This confirms we're designing an indexing machine, not a high-speed conveyor.

Step 5 — Required Force

The conveyor is horizontal.

The motor mainly overcomes:

friction
inertia
chain resistance

Instead of trying to calculate every friction source precisely, we'll use a conservative engineering estimate.

Assume:

Required tangential force:

5 N

This already includes a reasonable safety margin for a prototype.

Step 6 — Required Torque

Torque equation:

T=F×r

Where:

F = 5 N

r = 0.025 m

T=5×0.025
T=0.125Nm

Apply a safety factor of 3.

T
design
​

=0.375Nm

Final design requirement:

Minimum required shaft torque = 0.4 N·m

Step 7 — Compare Candidate Motors
Option A — NEMA 17 Stepper

Typical holding torque:

0.4–0.6 N·m

Advantages

Excellent positioning
No gearbox required
High repeatability
Easy indexing

Disadvantages

Higher power consumption
Can lose steps if overloaded
Requires stepper driver
Option B — JGY370 Worm Gear Motor

Depending on gearbox:

Typically:

0.8–5 N·m

Advantages

High torque
Self-locking gearbox
Lower cost
Quiet
Efficient for low-speed motion

Disadvantages

Position control requires encoder or sensors
Less precise than a stepper without feedback
Engineering Comparison
Parameter NEMA 17 JGY370
Meets Torque Requirement ✅ ✅
Precise Positioning ⭐⭐⭐⭐⭐ ⭐⭐⭐
Holding Position ⭐⭐⭐⭐ ⭐⭐⭐⭐⭐
Complexity Medium Low
Cost Medium Low
Power Consumption Higher Lower
Best for Indexing ⭐⭐⭐⭐⭐ ⭐⭐⭐⭐ (with position sensor)
Final Engineering Decision

This is an interesting outcome.

When we first discussed motors months ago, we were comparing them based largely on intuition.

Now we've calculated the requirements.

The numbers show that both motors provide more than enough torque for the estimated load.

The deciding factor is therefore control, not power.

For Version 1 (Prototype), I recommend:

JGY370 Worm Gear Motor + Position Sensor

Reason

It exceeds the required torque.
It operates naturally at low speed.
It is quieter and more economical.
With an IR or photoelectric position sensor at the weighing station, we can achieve repeatable indexing without the cost and complexity of a stepper system.
