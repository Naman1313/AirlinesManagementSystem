Airline Management System

✈️ Project Overview

The Airline Management System is a comprehensive desktop application designed to digitize and streamline the daily operations of an airline. It provides an intuitive Graphical User Interface (GUI) for airline staff to manage passenger records, flight schedules, ticket bookings, and cancellations efficiently. The system replaces manual paperwork with a centralized database, ensuring data accuracy and faster service.

✨ Key Features

Secure Login: Role-based authentication system to prevent unauthorized access.

Passenger Management: Register and view customer details including personal info and passport data.

Flight Operations: View real-time flight schedules, source, and destination details.

Ticket Booking: Interactive interface to search for flights and book tickets, generating a unique PNR.

Cancellation System: Cancel existing bookings and automatically update the database.

Journey Details: Retrieve travel history and status using PNR.

Boarding Pass Generation: Auto-generate printable boarding passes for passengers.

🛠️ Technologies Used

Programming Language: Java (JDK 17)

GUI Framework: Java Swing & AWT

Database: MySQL (Relational Database)

Database Connectivity: JDBC (Java Database Connectivity)

IDE: NetBeans / VS Code / Eclipse

📸 Screenshots

1. Login Screen

Secure authentication gate for the system.

2. Main Dashboard

Central hub to access all features like Booking, Cancellation, and Flight Info.

3. Ticket Booking

Interface to select source, destination, and book flights.

(Note: If images are not loading, please check the 'screenshots' folder in the repository.)

⚙️ Installation & Setup

Prerequisites

Java Development Kit (JDK 8 or higher)

MySQL Server (8.0 recommended)

NetBeans IDE or VS Code with Java Extension Pack

Steps to Run

Clone the Repository:

git clone [https://github.com/Naman1313/AirlinesManagementSystem.git](https://github.com/Naman1313/AirlinesManagementSystem.git)


Database Configuration:

Open your MySQL Workbench or Command Line.

Create the database and tables by executing the SQL commands provided in database_script.sql (or manually create the airline database).

Alternative:

CREATE DATABASE airline;
USE airline;
-- (Import tables for login, passenger, flight, reservation, cancel)


Connect the Application:

Open src/airlinemanagementsystem/Conn.java.

Update the DB_URL, DB_USER, and DB_PASS fields with your local MySQL credentials.

Run the Project:

Run Login.java as the main class to start the application.

🧪 Instructions for Testing

To verify the system functionality, use the following default credentials and test cases:

1. Login Test

Username: admin

Password: admin

Expected Result: System should grant access and open the Home Dashboard.

2. Database Connection Test

Navigate to "Flight Details" from the menu.

Expected Result: A table should appear listing the flights (e.g., "AI-1212" from Delhi to Mumbai). If the table is empty or shows an error, check your MySQL service.

3. Booking Flow Test

Go to "Book Flight".

Enter a valid Aadhar number (from a registered customer).

Select Source: Delhi and Destination: Mumbai.

Click "Book Flight".

Expected Result: A pop-up "Ticket Booked Successfully" should appear, and a new PNR is generated in the database.

🗂️ Database Schema

The system uses the following relational tables:

login: Stores admin credentials.

passenger: Stores personal details (Name, Address, Nationality, Gender).

flight: Stores flight codes, names, and routes.

reservation: Links passengers to flights with PNR, Ticket ID, and Date.

cancel: Archives details of cancelled tickets.

Developed by: Naman Chaudhary (24BCE10728)
