# Week 6 — Creating UML Class Diagrams 


## Part B — Identify domain concepts

### Task B1 — Find candidate concepts
| Candidate | Class, attribute or action? | Supporting requirement |
|:---------:|:---------------------------:|:-----------------------:|
| Student | Class | FR01 |
| Booking | Action | FR01, FR02, FR03 |
| Start date | Attribute of Booking | FR03 |
| Equipment | Class | FR02, FR05 |
| Review | Action / relationship | FR04 |
| Staff Member | Class | FR04, FR05 |

### Task B2 — Select the classes
• Student - A student uses the system to make equipment bookings.
• Booking - A booking records the equipment requested and the start and end dates.
• Equipment - Equipment shows the items that students can book.
• Staff Member - Staff members review booking requests and manage equipment availability.

### Task B3 — Identify uncertainty
A possible additional attribute is studentEmail.

## Part E — Multiplicity and requirements questions

### Task E3 — Record open questions

• Can one booking be associated with multiple students, or must every booking belong to exactly one student?
• Can the same equipment item be booked multiple times, and are overlapping booking dates allowed?
• Should the system store approval or rejection as a Booking status?

## Part F — Review your Class Diagram
### Task F1 — Requirements-to-model check
| Requirement | Where is it represented in the diagram? | Fully represented? |
|:-----------:|:---------------------------------------:|:------------------:|
| FR01 |Student–Booking relationship | FR01 | Partially |
| FR02 | Booking–Equipment relationship and 1 | Partially |
| FR03 | Booking attributes startDate and endDate  | Yes |
| FR04t | Staff Member–Booking relationship | Partially |
| FR05 | Staff Member–Equipment relationship | Partially |
| FR06 | Booking decision/status question | Needs clarification |

## Part G — New example: Campus Workshop Registration

### Task G1 — Identify classes
1. Student.
2. Registration.
3. Workshop.
### Task G2 — Identify attributes
| Class | Where is it represented in the diagram? | Fully represented? |
|:-----------:|:---------------------------------------:|:------------------:|
| Student | studentID, name | WR01 |
| Registration | registrationDate, status | WR07 |
| Workshop | workshopCode, title | WR02 |

### Task G4 — Add multiplicities
| Association | Multiplicity at first class | Multiplicity at second class |
|:-----------:|:---------------------------------------:|:------------------:|
| Student–Registration | |
| Registration–Workshop |
### Task G5 — Interpret the model
1. One Student can have zero or many Registration records.
2. Each Registration belongs to exactly one Student.
3. One Workshop can have zero or many Registration records.
4. Each Registration is for exactly one Workshop.

