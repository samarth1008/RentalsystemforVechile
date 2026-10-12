# Rental system for vehicle

## Project Description
The Rental system for vehicle is a Java-based console application that manages vehicles, customers, rentals, returns, billing, and rental history. It uses Object-Oriented Programming, ArrayList, methods, inheritance, polymorphism, and file handling.

## Features
- Add, display, search, and remove vehicles
- Support for Cars, Bikes, and other vehicles
- Add and search customers
- Rent and return vehicles
- Calculate rental bills
- Maintain rental history
- Save and load data using text files
- Menu-driven interaction
- Basic input validation

## Technologies and Concepts
- Java
- Classes and Objects
- Constructors
- Methods
- Inheritance
- Method Overriding
- Polymorphism
- Object Composition
- ArrayList / Collections
- File Handling (`FileWriter`, `FileReader`, `BufferedReader`)
- Exception Handling (`IOException`)

## Project Structure
```text
RentalsystemforVechile
├── src
│   ├── Main.java
│   ├── Vehicle.java
│   ├── Car.java
│   ├── Bike.java
│   ├── Customer.java
│   └── Rental.java
├── vehicles.txt
├── customers.txt
├── rentals.txt
├── Rental_system_for_vehicle_report.pdf
└── README.md
```

The source code is in the `src` folder. The three `.txt` files in the project root store the saved data, and the application reads and writes them from the folder it is run in.

## Main Classes
### Vehicle
Stores vehicle ID, brand, model, rent per day, and availability.

### Car
Extends `Vehicle` and adds the number of seats.

### Bike
Extends `Vehicle` and adds engine capacity in CC.

### Customer
Stores customer ID, name, and phone number.

### Rental
Connects a customer with a vehicle, stores rental duration, and calculates the total bill.

### Main
Contains the application flow, ArrayLists, menu, rental operations, searching, removal, and file handling.

## File Handling
The application stores data in:
- `vehicles.txt`
- `customers.txt`
- `rentals.txt`

Data is loaded when the application starts and is saved after each menu action. It can also be saved manually with the **Save Data** option.

## Menu
```text
1. Display Vehicles
2. Add Vehicle
3. Search Vehicle
4. Remove Vehicle
5. Add Customer
6. Search Customer
7. Rent Vehicle
8. Return Vehicle
9. Rental History
10. Save Data
11. Exit
```

## How to Run

**Requirements:** Java JDK 8 or higher.

**Option 1: Command line**

Open a terminal in the project's root folder (the folder that contains `src` and the `.txt` files) and run:

```bash
javac -d out src/*.java
java -cp out Main
```

Run these commands from the root folder so the program can find `vehicles.txt`, `customers.txt`, and `rentals.txt`.

**Option 2: IntelliJ IDEA**
1. Open the project folder in IntelliJ IDEA.
2. Make sure the `src` folder is marked as the Sources Root.
3. Run `Main.java`.

**Using the application**
1. Enter the number of a menu option and press Enter.
2. Choose option **11** to exit the program.

## OOP Concepts Demonstrated
- **Encapsulation:** Data and related operations are grouped inside classes.
- **Inheritance:** `Car` and `Bike` extend `Vehicle`.
- **Polymorphism:** A `Vehicle` reference can refer to a `Car` or `Bike`, with overridden `displayVehicle()` methods being invoked at runtime.
- **Composition:** `Rental` contains references to `Customer` and `Vehicle`.

## Author
**Samarth Mishra**

B.Tech CSE (AI & ML)  
VIT Bhopal
