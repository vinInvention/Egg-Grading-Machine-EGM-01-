Engineering Lesson #8

Every engineering system can be broken into subsystems.

Think of a car.

Car

↓

Engine

↓

Transmission

↓

Brakes

↓

Steering

↓

Electrical

↓

Cooling

No engineer designs the brakes before knowing where they fit in the whole system.

The same applies to EGM-01.

Step 1 — Define the Main Subsystems

I don't see EGM-01 as "a machine."

I see it as eight subsystems working together.

                EGM-01

                   │

──────────────────────────────────────

1. Feeding System

2. Conveyor System

3. Weighing System

4. Sorting System

5. Control System

6. User Interface

7. Power System

8. Structural System

Let's discuss each.

1. Feeding System

Purpose

Deliver one egg at a time to the conveyor.

Possible components

Feed tray
Hopper
Escapement mechanism
Guide rails

Input

Many eggs

Output

One egg

2. Conveyor System

Purpose

Transport eggs safely.

Components

Chain
Sprockets
Shafts
Bearings
Stepper motor
Egg holders

Input

One egg

Output

Egg at weighing station

3. Weighing System

Purpose

Determine egg weight.

Components

Load Cell
HX711
Weighing compartment

Input

One egg

Output

Weight in grams

4. Sorting System

Purpose

Place egg into correct tray.

Components

Servo
Push arm
Collection trays

Input

Egg category

Output

Egg sorted

5. Control System

Purpose

Coordinate everything.

Components

Arduino
Sensors
Motor driver
Servo driver

Responsibilities

Stop conveyor
Read weight
Decide category
Move servo
Count eggs 6. User Interface

Purpose

Communicate with operator.

Components

LCD
Buttons
LEDs
Buzzer

Displays

Current Weight

Category

Total Eggs

Machine Status

7. Power System

Purpose

Supply power safely.

Components

Power Supply
Battery
Fuse
Switch
Voltage regulators 8. Structural System

Purpose

Support everything.

Components

Frame

Legs

Motor mounts

Protective covers

Fasteners

Step 2 — Define the Machine Workflow

Now let's describe exactly how EGM-01 operates.

Operator loads eggs

↓

Egg enters hopper

↓

Escapement releases one egg

↓

Conveyor compartment receives egg

↓

Conveyor moves

↓

Egg reaches weighing station

↓

Stepper stops

↓

Load cell measures weight

↓

Arduino classifies egg

↓

Servo pushes egg

↓

Egg rolls into tray

↓

Counter increments

↓

Conveyor moves again

↓

Repeat
