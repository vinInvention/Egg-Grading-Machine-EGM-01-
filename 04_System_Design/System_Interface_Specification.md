# System Interface Specification (SIS)

# Project

Egg Grading Machine (EGM-01)

Version 1.0

---

# Purpose

This document defines how each subsystem within EGM-01 exchanges materials, signals, and information with other subsystems. Clear interface definitions allow each subsystem to be designed independently while ensuring complete system integration.

---

# Interface SI-001

## Feeding System → Conveyor System

Purpose

Transfer one egg safely into an empty conveyor compartment.

Input

Eggs from operator.

Output

Single egg positioned in conveyor holder.

Interface Type

Mechanical

Requirements

- Only one egg released at a time.
- No egg damage.
- No double feeding.

---

# Interface SI-002

## Conveyor System → Position Detection System

Purpose

Detect when a conveyor compartment reaches the weighing station.

Input

Moving conveyor compartment.

Output

Digital position signal.

Interface Type

Sensor

Requirements

- Detect every compartment.
- Ignore ambient light interference.
- Response time less than 100 ms.

---

# Interface SI-003

## Position Detection → Controller

Purpose

Notify the controller that an egg is ready for weighing.

Input

Digital HIGH/LOW signal.

Output

Interrupt or polling event.

Interface Type

Electrical

Requirements

- Reliable signal.
- Noise resistant.

---

# Interface SI-004

## Controller → Stepper Motor Driver

Purpose

Move or stop the conveyor.

Input

Motion command.

Output

Stepper pulses.

Interface Type

Electrical

Requirements

- Accurate positioning.
- Smooth acceleration.

---

# Interface SI-005

## Weighing System → Controller

Purpose

Transmit egg weight.

Input

Load cell signal.

Output

Weight in grams.

Interface Type

Electrical

Requirements

- Resolution better than 1 g.
- Stable reading before transmission.

---

# Interface SI-006

## Controller → Sorting System

Purpose

Command the servo to direct the egg into the correct tray.

Input

Egg category.

Output

Servo position.

Interface Type

Electrical

Requirements

- Correct tray selection.
- Complete movement before egg release.

---

# Interface SI-007

## Controller → User Interface

Purpose

Display machine status.

Information Displayed

- Weight
- Category
- Total eggs
- Machine state

Interface Type

Digital

---

# Interface SI-008

## Power System → All Subsystems

Purpose

Provide regulated electrical power.

Voltage Levels

- 12 V
- 5 V
- 3.3 V (if required)

Requirements

- Stable voltage.
- Overcurrent protection.
- Reverse polarity protection.
