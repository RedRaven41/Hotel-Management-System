# Project Statement

## Hotel Management System

**Student Name:** Tanishq Chaudhary
**Registration No.:** 25BAI10574

## 1. Problem Statement

Running a hotel on paper is slow and easy to get wrong. Room availability has to be tracked by hand, guest records get scattered across registers, reservations can be double-booked, and bills have to be worked out manually every time a guest checks out.

The Hotel Management System replaces that process with a Java-based console application. Staff can manage rooms, register guests, create and cancel bookings, generate bills, and check occupancy at a glance, all from one place.

## 2. Project Scope

The project targets the day-to-day operational needs of a hotel rather than trying to cover everything a large chain would require. It handles room management, guest management, bookings and cancellations, billing, and an occupancy dashboard, with input validation and error handling built in throughout.

This version runs as a console application and stores its data in CSV files.

## 3. Target Users

The system is meant for hotel administrators, reception staff, and general hotel employees, particularly at smaller hotels where a full commercial management suite would be more than what's needed. The interface is menu-driven, so it can be operated by anyone comfortable with a keyboard and a terminal.

## 4. High-Level Features

**Room Management** stores the details of each room: its number, type, price, and current availability status.

**Guest Management** keeps guest records including a guest ID, name, contact information, and other relevant details.

**Booking Management** lets staff create a reservation, pick from the rooms currently free, save the booking details, and cancel a reservation later. Room availability updates automatically whenever a booking is made or cancelled.

**Billing** works out the room charges, adds any service charges and tax, and produces the final amount payable.

**Dashboard** shows the total number of rooms, how many are free, how many are occupied, and the resulting occupancy figure for the hotel.

## 5. Technical Approach

The application uses a modular object-oriented design. The main classes are:

```text
Main
Room
Guest
Booking
Bill
Staff
FileManager
RoomManager
GuestManager
BookingManager
BillManager
ReportManager
InputValidator
```

The model classes (`Room`, `Guest`, `Booking`, `Bill`, `Staff`) represent the hotel's entities, while the manager classes handle the operations performed on them. `FileManager` takes care of reading from and writing to the CSV files, and `InputValidator` checks user input before it reaches the rest of the system, which keeps invalid data out.

## 6. Data Storage

All data lives in CSV files in the `data` directory:

```text
data/
├── rooms.csv
├── guests.csv
├── bookings.csv
├── bills.csv
└── staff.csv
```

Keeping storage file-based means there is no database server to install or configure, which makes the project straightforward to run for demonstrations and academic evaluation.

## 7. Expected Outcome

Once implemented, the system should give the user a working hotel management application: viewing and managing rooms, registering guests, creating and cancelling bookings, generating bills, checking hotel occupancy, and having all of that information saved to and reloaded from files between sessions.

## 8. Author Information

**Name:** Tanishq Chaudhary
**Registration No.:** 25BAI10574
**Project:** Hotel Management System
**Technology:** Java
