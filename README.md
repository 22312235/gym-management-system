# 🏋️ Gym Management System

## 📚 Course
CMPE314 – Software Engineering

## 👥 Team Members
- 22312235 Hana Shaimi
- 22310812 Majdoline ELBENNADI
- 22213379 Raid Idris

---

## 📌 Project Description
This project is a Gym Management System designed to manage gym members,
trainers, class schedules, and membership payments. The system aims to
simplify gym operations and improve user experience through a digital platform.

---

## 📊 Lab 1 – Gantt Chart
This section includes the initial project schedule showing tasks,
durations, and dependencies.



## 👨‍💻 Lab 2 – Resource Allocation
In this lab, team members were assigned to tasks based on their roles and skills.


### Resource Allocation Explanation
Tasks were assigned based on team members’ strengths:

- Hana: Requirements, testing, and documentation  
- Majdoline: UI/UX design and frontend development  
- Raid: Backend development, database, and deployment  

Some tasks such as API integration and bug fixing were shared among team members
to ensure collaboration and efficiency.

---
# 📊 Lab 3 – Use Case Diagrams

## 📌 Objective
The objective of this lab is to design and represent system functionality using UML Use Case Diagrams. It involves identifying actors, defining use cases, and modeling their interactions.

---

## 📍 Part 1: Gym Management System
A use case diagram was designed for the Gym Management System.

### Actors:
- Member
- Registered Member
- Receptionist
- Admin
- Payment System

### Main Use Cases:
- Browse Membership Plans
- Search Classes
- View Class Details
- Login
- Book Session
- Join Membership
- Renew Membership
- Checkout
- Process Payment
- Manage Members
- Manage Schedule
- Generate Reports

---

Lab 4 – Sequence Diagrams
Part 1 – Library Kiosk Sequence Diagram

The sequence diagram models the “Return Book” use case in the Library Kiosk system. The process begins when a student scans a book using the kiosk system. The system validates the book through the library database and checks whether the book is overdue.

If the book is overdue, the kiosk calculates the fine and requests payment before continuing the return process. After successful validation and payment, the inventory is updated, a confirmation notification is sent, and the book is placed back on the shelf.

Main Features
Normal return workflow
Overdue fine handling
Invalid book handling
Scanner failure alternative flow
Notification service interaction
Part 2 – Gym Management System Sequence Diagram

The Gym Management System sequence diagram models the interactions between the user, system components, and database during gym operations such as authentication, membership management, subscription handling, attendance tracking, and payment processing.

The diagram includes:

Login validation
Member/trainer management
Subscription and payment processing
Alternative validation flows
Lab 5 – Activity Diagrams
Part 1 – Library Kiosk Activity Diagram

The activity diagram models the workflow of returning a book through the library kiosk system. The process includes scanning the book, validating it, checking overdue status, calculating fines, and updating the inventory.

Decision nodes are used to handle:

Invalid books
Overdue books
Fine payment approval

Parallel activities are represented using fork and join nodes:

Updating inventory
Sending notifications
Returning the book to the shelf
Part 2 – Gym Management System Activity Diagram

The Gym Management System activity diagram models the administrator workflow inside the GymPro platform.

The workflow includes:

User authentication
Dashboard navigation
Member and trainer management
Subscription management
Payment recording
Logout and session clearing

Decision points validate user credentials and system actions, while management tasks can occur independently within the system.

Lab 6 – Data Flow Diagrams (DFDs)
Part 1 – Library Kiosk DFDs
Context Diagram (Level 0)

The Level 0 DFD represents the Library Kiosk Return Book System as a single process interacting with:

Student
Library Database
Notification Service
Shelf Mechanism

Main data flows include:

Book ID
Fine payment
Validation requests
Return confirmations
Level 1 DFD

The Level 1 DFD decomposes the Return Book System into multiple sub-processes:

Validate Book
Check Due Date
Process Fine
Update Inventory
Send Notification

The diagram also includes:

Book Inventory
Borrower Records
Transaction Log
Level 2 DFD

The Level 2 DFD expands the “Process Fine” sub-process into:

Calculate Fine
Present Fine to Student
Record Payment

It demonstrates how overdue information, payment details, and transaction records move through the system.

Part 2 – Gym Management System DFDs
Context Diagram (Level 0)

The Gym Management System context diagram models the interaction between:

Admin
Trainer
Member

and the central Gym Management System process.

Level 1 DFD

The Level 1 DFD decomposes the system into major processes:

Authenticate User
Manage Members/Trainers
Manage Assignments
Manage Subscriptions/Payments
Attendance and Reporting

The diagram also includes several data stores:

Users
Members
Trainers
Assignments
Subscriptions
Payments
Attendance
Level 2 DFD

The Level 2 DFD expands one selected process into detailed lower-level processes, showing:

Internal data movement
Database interactions
Fine-grained workflow operations
Repository Structure
/SequenceDiagrams
/ActivityDiagrams
/DFDDiagrams
/index.html
/style.css
/script.js
README.md
Technologies Used
HTML5
CSS3
JavaScript
PlantUML
Draw.io
GitHub Pages


