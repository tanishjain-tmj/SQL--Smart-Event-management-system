Smart Event Management System:

Project Overview:
The Smart Event Management System is a MySQL-based database project designed to manage events efficiently.
It enables event organizers to create and manage events, handle attendee registrations, track ticket bookings, process payments, and generate useful reports.
This project demonstrates the practical use of core and advanced SQL concepts, including CRUD operations, joins, subqueries, aggregate functions, window functions, and CASE expressions.

Objectives:
Manage events, venues, organizers, attendees, tickets, and payments
Track ticket sales and payment status
Generate insights like revenue, popular events, and demand levels
Apply SQL concepts required for academic practical exams and real-world systems

Database Schema:
The database consists of six interconnected tables with proper primary and foreign key relationships:
Events
Venues
Organizers
Attendees
Tickets
Payments
Relationships ensure data consistency and prevent duplicate or invalid records.

Table Description:
1. Events
Column Name
Description
event_id
Primary Key
event_name
Name of the event
event_date
Date of the event
venue_id
Foreign Key → Venues
organizer_id
Foreign Key → Organizers
ticket_price
Price per ticket
total_seats
Total seats available
available_seats
Seats remaining
2. Venues
Column Name
Description
venue_id
Primary Key
venue_name
Venue name
location
City/location
capacity
Maximum seating capacity
3. Organizers
Column Name
Description
organizer_id
Primary Key
organizer_name
Organizer name
contact_email
Email ID
phone_number
Contact number
4. Attendees
Column Name
Description
attendee_id
Primary Key
name
Attendee name
email
Email address
phone_number
Contact number
5. Tickets
Column Name
Description
ticket_id
Primary Key
event_id
Foreign Key → Events
attendee_id
Foreign Key → Attendees
booking_date
Ticket booking date
status
Confirmed / Cancelled / Pending
6. Payments
Column Name
Description
payment_id
Primary Key
ticket_id
Foreign Key → Tickets
amount_paid
Payment amount
payment_status
Success / Failed / Pending
payment_date
Date of payment

SQL Operations Covered:
CRUD Operations (INSERT, SELECT, UPDATE, DELETE)
SQL Clauses (WHERE, HAVING, LIMIT)
Logical Operators (AND, OR, NOT)
Sorting & Grouping (ORDER BY, GROUP BY)
Aggregate Functions (SUM, AVG, MAX, MIN, COUNT)
Joins (INNER, LEFT, RIGHT, FULL OUTER)
Subqueries
Date & Time Functions
String Functions
Window Functions
CASE Expressions
Primary & Foreign Key Constraints

Queries Implemented:
🔹 Basic Operations
Add, update, delete, and search records
Retrieve upcoming events by city
Find attendees who booked tickets recently
🔹 Aggregation & Reporting
Total revenue generated from all events
Event with the highest number of attendees
Average ticket price across events
Revenue generated per event
🔹 Joins & Relationships
Event details with venue information
Attendees who booked tickets but did not complete payment
Events with no attendees
Attendees who never booked any ticket
🔹 Subqueries
Events generating revenue above average ticket sales
Organizers managing more than a specific number of events
🔹 Date & Time Functions
Extract month from event date
Calculate days remaining for upcoming events
Format payment date
🔹 String Functions
Convert organizer names to uppercase
Trim extra spaces from attendee names
Replace NULL email values
🔹 Window Functions
Rank events based on total revenue
Cumulative ticket sales
Running total of attendees per event
🔹 CASE Expressions
Categorize events as High / Moderate / Low Demand
Classify payment status as Successful / Failed / Pending

Conclusion:
The Smart Event Management System successfully demonstrates how a relational database can be used to manage real-world event operations using SQL.
This project strengthens understanding of database design, relationships, and advanced SQL queries, making it suitable for academic practical exams, viva, and portfolio projects.
