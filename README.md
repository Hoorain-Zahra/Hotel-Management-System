# Hotel-Management-System
HotelSync - Hotel Management System
Project Overview:
HotelSync is a comprehensive hotel management system designed to streamline hotel operations, including customer management, staff coordination, room inventory, bookings, check-ins/check-outs, payments, services, and maintenance tracking. Built using PHP, MySQL, HTML, and JavaScript, this system provides an efficient and user-friendly interface for hotel administrators to manage daily operations.

Features:
Customer Management: Add, view, and update customer details such as name, phone, email, and address.
Staff Management: Manage staff information, including roles, contact details, and assignments.
Room Inventory: Track room details, including room number, type, rate, status, and floor.
Service Offerings: Manage hotel services like room service, laundry, and spa with associated charges.
Booking Management: Create and manage bookings with details like customer ID, room ID, booking date, check-in/check-out dates, and status.
Check-In/Check-Out Records: Record and track check-in and check-out activities with staff assignments and timestamps.
Payment Transactions: Process payments with support for multiple payment methods and status tracking.
Maintenance Logs: Log and track maintenance issues for rooms, including issue description, start/end dates, and status.
Database-Driven: Utilizes MySQL for robust data storage and retrieval, with prepared statements for security.
API Support: Provides a JSON-based API for fetching and adding records to various tables.
Responsive Dashboard: A user-friendly HTML interface for managing all aspects of the hotel operations.

Tech Stack:
Frontend: HTML, JavaScript
Backend: PHP
Database: MySQL
Libraries/Frameworks: PDO for database connectivity
Server: Compatible with Apache (e.g., XAMPP/WAMP)

File Structure:
index.html / index.php: Main dashboard and login interface for the system.
config.php: Database connection configuration using PDO.
api.php: Handles API requests for fetching and adding records to tables.
process_checkin.php: Processes check-in operations, updating booking and room statuses.
process_payment.php: Manages payment processing with transaction handling and status updates.
HMS MYSQL updated.sql: SQL script to create the database, tables, and populate sample data, along with example DML queries.

Database Schema:
The system uses a MySQL database (hotel_management_system) with the following tables:
customer: Stores customer information.
staff: Manages staff details.
rooms: Tracks room inventory.
services: Lists available hotel services.
bookings: Manages booking records with foreign keys to customer and rooms.
checkins: Records check-in details with references to bookings and staff.
checkouts: Tracks check-out details with references to bookings and staff.
payments: Manages payment transactions linked to bookings.
maintenance: Logs maintenance issues linked to rooms and staff.


Sample Queries
The HMS MYSQL updated.sql file includes sample DML queries, such as:
Fetching customers from a specific city (e.g., Lahore).
Listing available rooms.
Identifying bookings with pending payments.
Updating room rates or customer details.
Deleting old maintenance records.

Future Enhancements:
Add user authentication for secure login.
Implement update and delete operations in api.php.
Enhance the frontend with CSS frameworks (e.g., Bootstrap) for better UI/UX.
Add reporting features for analytics (e.g., revenue, occupancy rates).
Implement real-time notifications for staff assignments.
