# Functional Requirements Specification (FRS)

# Project

Egg Grading Machine (EGM-01)

Version: 1.0

---

# Purpose

This document defines the functional behaviour of the Egg Grading Machine (EGM-01). Functional requirements describe the actions the system must perform to satisfy the customer's needs.

---

# Functional Requirements

## FR-001 Egg Feeding

The machine shall allow the operator to place multiple eggs into a feed tray for continuous grading.

Priority: Must Have

Verification:
Demonstration

---

## FR-002 Egg Transportation

The machine shall transport eggs individually from the feed tray to the weighing station using a chain-driven conveyor.

Priority: Must Have

Verification:
Functional Test

---

## FR-003 Egg Positioning

The conveyor shall stop automatically when an egg reaches the weighing station.

Priority:
Must Have

Verification:
Functional Test

---

## FR-004 Weight Measurement

The machine shall measure the weight of each egg using a load cell.

Priority:
Must Have

Verification:
Calibration Test

---

## FR-005 Egg Classification

The controller shall classify eggs into predefined weight categories.

Priority:
Must Have

Verification:
Functional Test

---

## FR-006 Automatic Sorting

The machine shall actuate a servo-operated gate to direct each egg into the appropriate collection tray.

Priority:
Must Have

Verification:
Demonstration

---

## FR-007 Egg Counting

The system shall maintain a running count of all successfully graded eggs.

Priority:
Must Have

Verification:
Functional Test

---

## FR-008 Daily Statistics

The system shall store daily grading statistics.

Priority:
Should Have

Verification:
Demonstration

---

## FR-009 Display Information

The machine shall display:

- Current egg weight
- Egg category
- Total eggs graded
- Machine status

Priority:
Should Have

Verification:
Inspection

---

## FR-010 Start and Stop Operation

The operator shall be able to start and stop the grading process using dedicated controls.

Priority:
Must Have

Verification:
Demonstration

---

## FR-011 Emergency Stop

The machine shall immediately stop all motion when the emergency stop button is pressed.

Priority:
Must Have

Verification:
Safety Test

---

## FR-012 System Initialization

When powered on, the machine shall initialize all sensors and actuators before beginning operation.

Priority:
Should Have

Verification:
System Test

---

## FR-013 Fault Detection

The controller shall detect common operational faults such as:

- No egg present
- Conveyor jam
- Load cell error

Priority:
Could Have

Verification:
System Test

---

## FR-014 Data Export

The system shall export daily grading statistics to Microsoft Excel.

Priority:
Should Have

Verification:
Demonstration

---

## FR-015 Shutdown

The machine shall safely complete its current operation before shutting down.

Priority:
Should Have

Verification:
Functional Test
