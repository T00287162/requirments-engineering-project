# Week 3 — Requirements Analysis and Specification

## 1. Information from Week 2
• We moved towards requirements elicitation.
• Identified stakeholders; 
• Considered stakeholder needs and concerns;
• Identified unknown information; developed question;

## 2. Candidate Requirements
| Statement | Classification | Reason |
|:---------:|:--------------:|:------:|
| People are sometimes unsure whether a camera is available. | Problem/observation | Describes the problem of the system, not system should do |
| Technicians need to know what equipment is due back. | Stakeholder needs/concern | Tells the need of technicians without saying how |
| The system shall record the expected return date for each booking. | Candidate requirement | Tells what system should do |
| The college should build a mobile app. | Solution idea | Straight solution without any states |
| We assume all users will have a college login. | Assumption | Users assume the idea for the project |
| A lecturer wants reliable availability information before promising equipment. | Stakeholder needs/concern | States what lecturer wants from system |
## 3. Requirements Surgery

### Requirement 1 - “The system shall be user-friendly.”
Very vague. User friendly means different things for different group of people.
#### What is the problem?
Users may find it difficult to interact with UI of the system.
#### One clarification question
Who is going to use the system and which tasks is going to be asked to complete.
#### What information is missing?
User groups, tasks.

### Requirement 2 - “The system shall notify users about bookings.”
#### What is the problem?
Doesn't say who is going to be notified, about what, when and how.
#### One clarification question
Which tasks will target the system to notify user, and who should receive it.
#### What information is missing?
Target events, notification recipient, timing. 

### Requirement 3 - “The system shall allow staff to create, edit and delete bookings and send reminders.”
#### What is the problem?
Statement "Staff" is not clear. A lot of action bundled into one.
#### One clarification question
Who is going to create, edit and delete bookings.
#### What information is missing?
Clarifying "staff" statement, what is "delete" means, group of users.

### Improved requirement (from Requirement 2)
Original: "The system shall notify users about bookings."
Improved: "The system shall notify borrower when there is deadline, change or cancel of the booking."
#### WHO?
The borrower.
#### WHAT?
Notification.
#### WHEN?
On confirmation, change, removal, deadline of the booking.
#### HOW WILL WE KNOW?
Confirm, change and cancel a test booking and check a notification is sent each time.

## 4. Functional Requirements
#### Who needs this?
Technicians
#### What does the system need to do?
View whether equipment is available.
#### When does a condition apply?
Before confirming a booking, for a selected date.
#### Why is this needed?
To avoid double-booking and to give reliable answers.
#### How could we verify it?
Select a date with known bookings and check that the availability shown is correct.

| ID | Requirement | Source | How could we verify it? |
|:--:|:-----------:|:------:|:-----------------------:|
| FR-01 | The system shall allow an authorised user to view equipment availability for a selected date. | Technician need | Select a date with known bookings and check that the availability shown is correct. |
| FR-02 | The system should record the expected return date for each booking. | Candidate requirement | Create a booking and check the return date is stored and displayed. |
| FR-03 | The system should allow a technician to view the equipment to the back on a selected date. | Technician need | Create bookings with different return dates and check only the items due on the selected date are listed. |

### Review the functional requirements
• FR-01: Behaviour is clear. "Authorised user" is not defined, so this is an unknown. We have assumed availability is checked per date rather than per time slot, which also needs confirming.
• FR-02: Clear and verifiable. Missing: whether the return date can be changed later and who may change it.
• FR-03: Clear and verifiable. Missing: how overdue items are shown, which is not covered yet.

## 5. Quality Requirements
| ID | Quality requirement | Why does it matter? | How could it be checked? |
|:--:|:-------------------:|:-------------------:|:------------------------:|
| NFR-01 | The system should allow only authenticated, authorised users to create, edit or cancel bookings. | Unauthorised changes could cause booking conflicts or loss of equipment. | Have access to these actions without logging in and with an unauthorised role, and confirm both attempts to access are refused. |
## 6. Project Application

## 7. Reflection
### 1. What makes a requirement difficult to understand? 
Vague words such as "efficiently" or "user-friendly", unclear actors such as "staff" or "users", several requirements bundled into one, and missing conditions. If a requirement cannot be verified, it is hard to know what it actually means.

### 2. What information do you still need for your project?
