# Conveyor System Research

## Project

Egg Grading Machine (EGM-01)

---

## Purpose

This study evaluates possible mechanisms for transporting eggs through EGM-01. The selected mechanism must transport eggs reliably, maintain accurate positioning at the weighing station, minimize egg damage, and remain affordable and maintainable for a small-scale poultry operation.

---

# Design Requirements

The conveyor system should:

- Transport eggs from the feeding system to the weighing station.
- Maintain predictable egg positioning.
- Minimize egg movement and impact.
- Support repeated start-stop operation.
- Operate at a suitable speed for the grading process.
- Be easy to maintain.
- Be affordable to fabricate.
- Allow future modification.

---

# Design Alternatives

## Option 1: Chain Conveyor with Individual Egg Holders

### Description

Two parallel chains are driven by sprockets mounted on shafts. Individual egg holders or compartments are attached between the chains.

The conveyor transports each egg in a controlled compartment.

### Advantages

- Positive mechanical drive.
- Minimal slippage.
- Precise compartment positioning.
- Suitable for indexing operation.
- Individual eggs can be isolated from one another.
- Compatible with a stepper motor.

### Disadvantages

- Requires careful alignment.
- Requires lubrication and maintenance.
- Chain tension must be controlled.
- Poorly designed holders may damage eggs.

---

## Option 2: Timing Belt Conveyor

### Description

A toothed belt transports eggs using attached holders or carriers.

### Advantages

- Quiet operation.
- Low maintenance.
- Good positional accuracy.
- Smooth movement.

### Disadvantages

- May be more expensive.
- Custom egg holders may be more difficult to fabricate.
- Belt material and attachment method require careful selection.

---

## Option 3: Flat Belt Conveyor

### Description

A continuous belt transports eggs along a flat surface.

### Advantages

- Simple design.
- Easy to construct.
- Widely available components.

### Disadvantages

- Eggs may roll or collide.
- Difficult to position a single egg accurately.
- Requires additional mechanisms for weighing and spacing.
- Greater risk of uncontrolled egg movement.

---

## Option 4: Roller Conveyor

### Description

Eggs are transported over rotating rollers.

### Advantages

- Simple mechanical concept.
- Can transport multiple eggs.

### Disadvantages

- Difficult to control individual egg position.
- Eggs may roll into one another.
- Less suitable for precise weighing.
- Higher risk of collisions.

---

# Comparison Matrix

| Criterion               | Chain with Holders | Timing Belt | Flat Belt | Roller Conveyor |
| ----------------------- | -----------------: | ----------: | --------: | --------------: |
| Precise Positioning     |               High |        High |    Medium |             Low |
| Egg Protection          |               High |        High |    Medium |             Low |
| Start-Stop Operation    |               High |        High |    Medium |          Medium |
| Construction Simplicity |             Medium |      Medium |      High |          Medium |
| Maintenance             |             Medium |        High |      High |            High |
| Cost                    |             Medium |      Medium |       Low |          Medium |
| Suitability for EGM-01  |               High |        High |    Medium |             Low |

---

# Engineering Analysis

The primary challenge in EGM-01 is not simply transporting eggs from one location to another.

The conveyor must also:

1. Receive one egg.
2. Maintain the egg in a controlled position.
3. Transport the egg to the weighing station.
4. Stop or position the egg accurately.
5. Allow the egg to be removed after weighing.
6. Continue operating with the next egg.

This makes a compartment-based transport system more appropriate than a simple continuous belt.

---

# Preliminary Selection

The chain conveyor with individual egg holders is currently the preferred concept for EGM-01.

The design consists of:

- Two parallel chains.
- Two drive sprockets on a common shaft.
- Two driven sprockets on a second shaft.
- Individual egg holders attached between the chains.
- A motor connected to the drive shaft.

```text
        DRIVE SHAFT                         IDLER SHAFT
     ┌─────────────┐                     ┌─────────────┐
     │  Sprocket 1 │=====================│ Sprocket 1  │
     │             │      Chain 1        │             │
     │  Sprocket 2 │=====================│ Sprocket 2  │
     └─────────────┘      Chain 2        └─────────────┘
             │
             │
        Motor Drive
```
