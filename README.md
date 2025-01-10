
```markdown
# Project Title
Equipment-Rental-System

## Description
This project is a Java application designed to manage club equipment and members. Users can borrow equipment, verify member statuses, and handle reservations. The application utilizes object-oriented programming (OOP) principles, which enhances code reusability and maintainability.

The system implements interfaces to set contracts for various commands, allowing for seamless integration and management of different command implementations. A significant focus is placed on error handling, with custom exceptions created to manage scenarios such as member not found, equipment already borrowed, and invalid input. This comprehensive error handling approach improves user experience by offering clear feedback and preventing system crashes.

## Features
-Member registration and management
-Equipment creation and management
-Borrowing and requesting equipment
-Tracking equipment availability and borrowing history
-Member status and borrowing history tracking
-Undo and redo functionality for borrowing and requesting equipment

## Installation
1. Ensure that the Java Development Kit (JDK) is installed on your machine.
2. Clone the repository using:
```
git clone https://github.com/muhammadmahad4/Equipment-Rental-System.git
```
3. Navigate to the project directory:
```
cd Equipment-Rental-System
```

## Usage
To run the application, compile the Java files and execute the `Main` class:
```
javac *.java
java Main
```
Follow the instructions displayed on-screen to interact with the application.

## File Structure
```
.
├── BorrowStatus.java
├── Club.java
├── CmdArrive.java
├── CmdBorrow.java
├── CmdCreate.java
├── CmdListEquipment.java
├── CmdListEquipmentStatus.java
├── CmdListMembers.java
├── CmdListMemberStatus.java
├── CmdRegister.java
├── CmdRequest.java
├── CmdStartNewDay.java
├── Command.java
├── Day.java
├── Equipment.java
├── EquipmentSet.java
├── ExEmployeeNotFound.java
├── ExEquipmentCodeAlreadyInUse.java
├── ExEquipmentRecordNotFound.java
├── ExIncorrectNumberOfDays.java
├── ExInsufficientArguments.java
├── ExInvalidDate.java
├── ExMemberAlreadyBorrowing.java
├── ExMemberIdAlreadyInUse.java
├── ExMemberNotFound.java
├── ExMemberNotUsingThisEquipment.java
├── ExMissingEquipmentRecord.java
├── ExNoAvailableSet.java
├── ExOverlapBorrow.java
├── ExOverlapRequest.java
├── ExUnknownCommand.java
├── Main.java
├── Member.java
├── RecordedCommand.java
├── RequestStatus.java
├── Reservation.java
├── Status.java
├── SystemDate.java
└── TextFiles/
    ├── 1c.txt
    ├── 1d.txt
    ├── 1d1.txt
    ├── 1d2.txt
    ├── 1d3.txt
    ├── 1e.txt
    ├── 1e1.txt
    ├── 2a.txt
    ├── 2b.txt
    ├── 2c.txt
    ├── 2x.txt
    ├── 3a.txt
    ├── 3b.txt
    ├── 3c.txt
    ├── 3c4.txt
```

## Commands
- **Borrow**: Enables a member to borrow equipment for a specified duration.
- **Create**: Adds a new equipment record to the system.
- **ListEquipment**: Displays all equipment currently available in the club.
- **ListMembers**: Shows all registered members within the club.
- **Register**: Registers a new member in the club.
- **Request**: Manages equipment requests, detailing the request date and duration.
- **StartNewDay**: Updates the current date in the system.
- **Arrive**: Marks equipment as returned in the system.
- **ListEquipmentStatus**: Provides the status of all equipment in the club.
- **ListMemberStatus**: Displays the status of all members in the club.

## Errors
- **ExInsufficientArguments**: Triggered when a command lacks sufficient arguments.
- **ExMemberNotFound**: Triggered when a specified member cannot be located in the system.
- **ExEquipmentRecordNotFound**: Triggered when a specified equipment record is missing.
- **ExMemberAlreadyBorrowing**: Triggered when a member tries to borrow equipment they already have.
- **ExOverlapBorrow**: Triggered when a borrowing period conflicts with an existing one.
- **ExNoAvailableSet**: Triggered when no equipment sets are available for borrowing.
- **ExInvalidDate**: Triggered when an invalid date is entered.
- **ExIncorrectNumberOfDays**: Triggered when the requested borrowing duration is invalid.
- **ExEquipmentCodeAlreadyInUse**: Triggered when attempting to create an equipment record with a duplicate code.
- **ExMissingEquipmentRecord**: Triggered when an expected equipment record is absent.
- **ExUnknownCommand**: Triggered when an unrecognized command is issued.
- **ExMemberIdAlreadyInUse**: Triggered when trying to register a member with a duplicate ID.
- **ExMemberNotUsingThisEquipment**: Triggered when a member is not associated with the specified equipment.
- **ExOverlapRequest**: Triggered when a request period conflicts with an existing borrowing/request period.

