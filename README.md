# Hotel Management System

A console-based Java application for managing hotel rooms, guests, bookings, billing, and reports.

## Project Information

**Student Name:** Sagan Gangwar
**Registration No.:** 25BAI10057
**Project:** Hotel Management System
**Language:** Java
**Type:** Console-Based Application

## About the Project

This is a Hotel Management System built in Java to handle the everyday tasks a small hotel deals with: keeping track of rooms, registering guests, making and cancelling bookings, generating bills, and pulling up reports.

The application is built around object-oriented design, with separate manager classes handling each part of the system. Data is stored in plain CSV files, so the project runs without any database setup. Input validation and exception handling are built in throughout, so bad input doesn't crash the program.

## Features

The system covers room management, guest management, booking creation and cancellation, billing, a dashboard showing current occupancy, and reports on hotel operations. Everything is saved to CSV files between runs, and all user input is validated before being processed.

## Technologies Used

Java forms the core of the project, using object-oriented programming, file handling, collections, and exception handling. Data persistence is handled with CSV files. The project can be opened in VS Code, IntelliJ IDEA, or Eclipse, and is version-controlled with Git and GitHub.

## Project Structure

```
HotelManagementJavaProject/
│
├── src/
│   └── hotelmanagement/
│       ├── Main.java
│       ├── Room.java
│       ├── Guest.java
│       ├── Booking.java
│       ├── Bill.java
│       ├── Staff.java
│       ├── FileManager.java
│       ├── RoomManager.java
│       ├── GuestManager.java
│       ├── BookingManager.java
│       ├── BillManager.java
│       ├── ReportManager.java
│       └── InputValidator.java
│
├── data/
│   ├── rooms.csv
│   ├── guests.csv
│   ├── bookings.csv
│   ├── bills.csv
│   └── staff.csv
│
├── docs/
│   ├── TestCases.md
│   ├── Design.md
│   ├── architecture.mmd
│   ├── usecase.mmd
│   ├── workflow.mmd
│   ├── sequence.mmd
│   └── class-diagram.mmd
│
├── README.md
├── statement.md
└── Hotel_Management_Project_Report.pdf
```

## Requirements

You'll need JDK 17 or later and a terminal. The project runs on Windows, Linux, and macOS. An IDE is optional. Around 4 GB of RAM and 500 MB of free storage is enough.

## How to Run

Open the project folder:

```
cd C:\Users\sagan\Downloads\HotelManagementJavaProject
```

Create the output folder:

```
mkdir out
```

Compile the project:

```
javac -d out src\hotelmanagement\*.java
```

Run the application:

```
java -cp out hotelmanagement.Main
```

## Application Modules

**Room Management** lets you add, view, and update hotel rooms, and check which ones are currently available.

**Guest Management** handles registering new guests and looking up or updating existing guest details.

**Booking Management** covers creating reservations and cancelling them when needed.

**Billing** calculates room charges, service charges, tax, and produces the final amount due.

**Dashboard** gives a quick view of current occupancy and room availability.

**Reports** pulls together information about how the hotel is running.

## Data Storage

All data is kept in CSV files inside the `data/` folder:

```
data/
├── rooms.csv
├── guests.csv
├── bookings.csv
├── bills.csv
└── staff.csv
```

No external database is required to run the project.

## Testing

Test cases cover room management, guest registration, booking creation and cancellation, billing, invalid input handling, room availability checks, dashboard calculations, and file persistence.

## Project Objectives

The goal was to build a working Hotel Management System in Java while applying object-oriented programming concepts in a practical setting. That meant implementing file handling and data persistence, managing rooms and guests, handling bookings and cancellations, generating bills, and adding proper input validation and error handling — all structured so the code stays modular and maintainable.

## Future Enhancements

There's plenty of room to grow this project. A graphical interface would make it far easier to use, and moving from CSV files to a MySQL database would handle larger volumes of data. Login and authentication with separate admin and staff roles would be a natural next step, along with online booking, payment gateway integration, and email or SMS confirmations. Further out, more advanced analytics and cloud deployment are both possible.

## Author

Sagan Gangwar
Registration No.: 25BAI10057

## License

This project was developed for academic and educational purposes.
