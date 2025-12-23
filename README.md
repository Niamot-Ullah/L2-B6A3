🚗 Vehicle Rental System – Database Design & SQL Queries
📌 Project Overview

This project is a Vehicle Rental System database designed to demonstrate understanding of:

Relational database design

Entity Relationship Diagram (ERD)

Primary and foreign keys

SQL queries using JOIN, EXISTS, WHERE, GROUP BY and HAVING

The system manages users, vehicles, and bookings, following real-world rental business logic.

🗂️ Database Structure

The database consists of three main tables:

1. Users

Stores user information such as:

Name, email, password, phone number

User role (Admin or Customer)

Each email is unique

2. Vehicles

Stores vehicle-related data including:

Vehicle name, type (car/bike/truck), model

Registration number (unique)

Rental price per day

Availability status (available, rented, maintenance)

3. Bookings

Stores booking details:

Which user made the booking

Which vehicle was booked

Rental start and end dates

Booking status (pending, confirmed, completed, cancelled)

Total booking cost

🔗 Entity Relationship Diagram (ERD)

One-to-Many: One user can have many bookings

Many-to-One: Many bookings can refer to one vehicle

Each booking connects exactly one user and one vehicle

The ERD was created using the drawSQL tool and includes:

Primary keys (PK)

Foreign keys (FK)

Relationship cardinality

Status fields for business logic

📄 SQL Queries (queries.sql)

All required SQL queries are written and stored in the queries.sql file.
Each query solves a specific requirement of the system.

Query 1: Retrieve Booking Information

Uses INNER JOIN to retrieve:

Booking details

Customer name

Vehicle name

Query 2: Vehicles Never Booked

Uses NOT EXISTS to find vehicles that have never been booked.

Query 3: Available Vehicles by Type

Uses WHERE clause to retrieve all available vehicles of a specific type (e.g., cars).

Query 4: Vehicles with More Than Two Bookings

Uses GROUP BY and HAVING to:

Count total bookings per vehicle

Display only vehicles with more than two bookings

✔ All queries are written correctly and follow the assignment requirements.

🧪 Technologies Used

PostgreSQL / SQL

drawSQL (for ERD design)

✅ Conclusion

This project successfully demonstrates:

Proper database design

Correct use of relational concepts

Efficient SQL querying techniques

All requirements mentioned in the assignment have been implemented and documented properly.
