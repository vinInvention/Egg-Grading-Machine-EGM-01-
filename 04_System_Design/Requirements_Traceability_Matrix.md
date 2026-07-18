# Requirements Traceability Matrix (RTM)

## Project

Egg Grading Machine (EGM-01)

---

## Purpose

The Requirements Traceability Matrix (RTM) provides a structured method for tracking every project requirement from its source through design, implementation, and testing. It ensures that all customer needs are addressed and that every implemented feature can be verified.

---

| ID      | Requirement                           | Source                  | Design Solution                  | Verification Method    | Status  |
| ------- | ------------------------------------- | ----------------------- | -------------------------------- | ---------------------- | ------- |
| FR-001  | Transport eggs automatically          | Mrs. B                  | Chain conveyor                   | Functional Test        | Pending |
| FR-002  | Measure egg weight                    | Mrs. B                  | Load Cell + HX711                | Calibration Test       | Pending |
| FR-003  | Classify eggs by weight               | Mrs. B                  | Arduino Classification Algorithm | Functional Test        | Pending |
| FR-004  | Sort eggs automatically               | Mrs. B                  | Servo Sorting Gate               | Demonstration          | Pending |
| FR-005  | Hold at least 5 eggs in the feed tray | Design Requirement      | Feed Tray Design                 | Inspection             | Pending |
| FR-006  | Count graded eggs                     | Mrs. B                  | Embedded Software Counter        | Functional Test        | Pending |
| FR-007  | Record daily grading statistics       | Design Requirement      | Excel Data Logging               | Demonstration          | Pending |
| NFR-001 | Operate without Internet              | Mrs. B                  | Standalone Embedded System       | System Test            | Pending |
| NFR-002 | Operate using backup power            | Mrs. B                  | Battery Backup System            | Power Failure Test     | Pending |
| NFR-003 | Minimize egg breakage                 | Mrs. B                  | Egg Holder & Conveyor Design     | Practical Test         | Pending |
| NFR-004 | Easy to operate                       | Stakeholder Analysis    | Simple User Interface            | User Evaluation        | Pending |
| NFR-005 | Easy to maintain                      | Stakeholder Analysis    | Modular Mechanical Design        | Maintenance Inspection | Pending |
| NFR-006 | Safe for operators                    | Engineering Requirement | Safety Guards & Emergency Stop   | Safety Inspection      | Pending |

---

## Notes

- Requirements may be updated as the project evolves.
- Verification methods will be completed during the testing phase.
- Status values will be updated throughout the project lifecycle.

Status Definitions:

- Pending
- In Progress
- Verified
- Failed
- Updated
