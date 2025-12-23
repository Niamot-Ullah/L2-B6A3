# Vehicle Rental System – Database Design & SQL Queries

## Project Description
This project implements a simplified **Vehicle Rental System** database to demonstrate understanding of:

- Relational database design
- Entity Relationship Diagrams (ERD)
- Primary keys and foreign keys
- SQL queries using JOIN, EXISTS, WHERE, GROUP BY, and HAVING

The system manages users, vehicles, and bookings following real-world rental business logic.

---

## Database Schema Overview
The database consists of three tables:

### Users
- Stores user information such as name, email, password, phone number
- Each user has a role (Admin or Customer)
- Email addresses are unique

### Vehicles
- Stores vehicle details such as name, type, model
- Each vehicle has a unique registration number
- Tracks rental price per day and availability status

### Bookings
- Stores booking records
- Links users and vehicles using foreign keys
- Contains rental period, booking status, and total cost

---

## Entity Relationship Diagram (ERD)
- One user can make multiple bookings (One-to-Many)
- A vehicle can appear in multiple bookings over time (Many-to-One)
- Each booking is associated with exactly one user and one vehicle

The ERD was created using the **drawSQL** tool and includes:
- Primary Keys (PK)
- Foreign Keys (FK)
- Relationship cardinality
- Status fields

---

## SQL Queries (`queries.sql`)
All required SQL queries are included in the `queries.sql` file.  
Each query directly solves a specific requirement of the assignment.

### Included Queries
1. **INNER JOIN**
   - Retrieves booking information along with customer name and vehicle name

2. **NOT EXISTS**
   - Finds vehicles that have never been booked

3. **WHERE Clause**
   - Retrieves all available vehicles of a specific type (e.g., cars)

4. **GROUP BY and HAVING**
   - Finds vehicles that have more than two bookings

Each query is written using proper SQL standards and comments for clarity.

---

## Submission Links
> Update the links below before final submission.

- **ERD Diagram (drawSQL):** [https://your-erd-link-here](https://drawsql.app/teams/car-booking/diagrams/car-booking)
- **GitHub Repository:** https://github.com/Niamot-Ullah/B2A3
- **queries.sql File:** https://your-queries-file-link-here

---

## Technologies Used
- SQL (PostgreSQL compatible)
- drawSQL (ERD design)

---

## Conclusion
This project fulfills all assignment requirements by combining proper database design with correctly implemented SQL queries.  
The documentation and queries demonstrate a clear understanding of relational databases and SQL concepts.
