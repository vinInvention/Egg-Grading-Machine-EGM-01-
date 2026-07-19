# Chain and Sprocket Selection Study

## Project

Egg Grading Machine (EGM-01)

Version 1.0

---

# Purpose

This study evaluates different chain sizes and sprocket configurations for the conveyor system. The selected chain must provide sufficient strength, accurate positioning, low maintenance, and compatibility with locally available components.

---

# Design Requirements

The chain system shall:

- Transmit conveyor motion without slipping.
- Support the combined weight of carriers and eggs.
- Allow indexing operation.
- Be easy to replace.
- Be readily available locally.
- Operate at low speed.
- Require minimal maintenance.

---

# Candidate Chains

## Option 1 — ANSI #25 Roller Chain

Pitch

6.35 mm

Advantages

- Lightweight
- Compact
- Low inertia
- Low cost

Disadvantages

- Lower load capacity
- Smaller sprockets may wear faster

---

## Option 2 — ANSI #35 Roller Chain

Pitch

9.525 mm

Advantages

- Good balance of strength and size
- Widely available
- Moderate weight

Disadvantages

- Slightly heavier than #25

---

## Option 3 — ANSI #40 Roller Chain

Pitch

12.7 mm

Advantages

- High strength
- Very common
- Durable

Disadvantages

- Heavy
- Larger sprockets
- More inertia than required

---

# Comparison Matrix

| Criteria               |      #25 |       #35 |       #40 |
| ---------------------- | -------: | --------: | --------: |
| Strength               |   Medium |      High | Very High |
| Weight                 | Very Low |       Low |      High |
| Cost                   |      Low |    Medium |    Medium |
| Availability           |   Medium |      High |      High |
| Suitable for Prototype |     High | Very High |    Medium |
| Oversized for EGM-01   |       No |        No |       Yes |

---

# Engineering Analysis

The estimated moving mass of the conveyor system is approximately 2.5 kg.

The required shaft torque is approximately 0.4 N·m after applying a safety factor.

All three candidate chains provide sufficient strength for this application.

Therefore, the decision should prioritize:

- Weight
- Cost
- Availability
- Ease of maintenance

rather than maximum strength.

---

# Sprocket Selection

Candidate tooth counts:

- 10 teeth
- 12 teeth
- 15 teeth
- 18 teeth

Engineering considerations:

- Smaller sprockets reduce machine size but increase chain articulation and wear.
- Larger sprockets reduce wear and produce smoother motion but increase machine dimensions.

A 15-tooth sprocket provides a good balance between compactness and smooth operation.

---

# Final Engineering Decision

## Selected Chain

ANSI #35 Roller Chain

## Selected Sprocket

15-tooth sprocket

## Reason

The ANSI #35 chain offers sufficient strength while maintaining moderate weight and good availability. A 15-tooth sprocket reduces chain wear compared to smaller sprockets and provides smoother indexing motion.

## Advantages

- Adequate strength
- Reduced inertia
- Easy to source
- Good durability
- Compact design

## Disadvantages

- Slightly larger than #25 chain
- Higher cost than #25

## Future Considerations

Future versions may investigate:

- Stainless steel chains
- Plastic tabletop chains
- Food-grade modular conveyor chains
