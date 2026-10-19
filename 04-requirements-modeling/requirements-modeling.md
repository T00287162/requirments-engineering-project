## Week 4 — Requirements Modelling
## Requirement used

• FR-01: The system shall allow an authorised user to view equipment availability for a selected date.

• FR-02: The system shall record the expected return date for each booking.

|   | FR-01 | FR-02 |
|:-:|:-----:|:-----:|
| Is it a requirement? | Yes, it says what the system should do and can be verified | Yes, it can be verified|
| Goal | See whether equipment is available on a chosen date | Have the expected return date stored with each booking. |
| Use case name | View Equipment Availability | Record Expected Return Date |
| Actor established? | "Authorised user" is not defined | No |
| Clarification question | Which roles count as "authorised users" for viewing availability? | Who records the expected return date? |

## Actors

• Student

• Equipment Technician

## Use Cases

• View aviability

• Create Booking

• Record return

• Record expected return date

## Modelling problem

| Example | What is wrong? |
|:-------:|:--------------:|
| Database drawn as an actor | Database is a part of the system, not a stakeholder |
| Booking Screen drawn as a use case | A booking screen is a interface element. |
| Student placed inside the system boundary | Actors are external to the system and belong outside the boundary. |
| "Do Stuff" used as a use case name | Too vague, the case name needs to be more clarified |
| Every stakeholder added as an actor | Only roles that directly interacts with the system are actors. |

## Unknowns / Questions

• Which roles are "authorised users"?

• Who records expected return date?

• Does the student also record the return date, or only technician?

• Can a Lecturer or Administrator create bookings?


## Reflection
• Diagrams helped me understand which roles interact with different actions.

• The requirement for the expected return date does not say who enters it.
