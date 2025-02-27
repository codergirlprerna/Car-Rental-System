# Car Rental System  

![alt text](<DALL·E 2025-02-27 15.31.10 - A modern car rental system concept illustration. The image features a digital platform interface with a customer selecting a car from available option.webp>)
## Overview
This is a simple **Car Rental System** implemented in Java, which allows customers to rent and return cars. The system keeps track of available cars, customers, and rentals.

---

## Features
1. **Add Cars to the System**  
   - Stores details like car ID, brand, model, base rental price, and availability status.

2. **Rent a Car**  
   - Customers can rent an available car for a specific number of days.
   - The total rental price is calculated based on the number of days.
   - Once rented, the car is marked as unavailable.

3. **Return a Car**  
   - Customers can return a rented car.
   - The car is marked as available again.
   - The rental record is removed.

4. **Simple CLI-Based Menu**  
   - Users can interact via a command-line menu to rent or return cars.

---

## Code Explanation

### **Car Class**
- Represents a car with attributes:
  - `carId`: Unique identifier for the car.
  - `brand`: Car brand (e.g., Toyota, Honda).
  - `model`: Car model.
  - `basePricePerDay`: Daily rental cost.
  - `isAvailable`: Availability status of the car.
- Methods:
  - `calculatePrice(int days)`: Computes rental price.
  - `rent()`: Marks the car as rented.
  - `returnCar()`: Marks the car as available.

### **Customer Class**
- Represents a customer with:
  - `customerId`: Unique customer identifier.
  - `name`: Customer's name.

### **Rental Class**
- Represents a rental transaction:
  - `car`: The rented car.
  - `customer`: The customer who rented the car.
  - `days`: Number of days for the rental.

### **CarRentalSystem Class**
- Manages the car rental operations.
- Attributes:
  - `cars`: List of available cars.
  - `customers`: List of registered customers.
  - `rentals`: List of ongoing rentals.
- Methods:
  - `addCar(Car car)`: Adds a new car to the system.
  - `addCustomer(Customer customer)`: Registers a new customer.
  - `rentCar(Car car, Customer customer, int days)`: Rents a car if available.
  - `returnCar(Car car)`: Returns a rented car.

### **Menu System (CLI)**
- Allows users to:
  1. **Rent a Car**: Displays available cars, takes customer input, and processes the rental.
  2. **Return a Car**: Allows a customer to return a car.
  3. **Exit**: Ends the program.

### **Main Class**
- Creates instances of `CarRentalSystem`, adds sample cars, and initiates the CLI menu.

---

## How to Run the Project
1. **Compile the Java Files**
   ```
   javac CarRentalSystem.java
   ```
2. **Run the Program**
   ```
   java CarRentalSystem
   ```
3. **Follow the On-Screen Menu** to rent or return cars.

---

## Issues & Fixes
### **Bugs in the Given Code**
- `menu()` is outside the `CarRentalSystem` class.
- `Car SelectedCar` should be `Car selectedCar`.
- `System.out.println("Total Price: $%.2f%n", totalPrice);` should be formatted using `String.format()`.

---

## Future Enhancements
- Implement a database for persistent storage.
- Add user authentication.
- Introduce different pricing models.

---


## 📌 Project Overview  
The **Car Rental System** is a simple **console-based Java application** that allows users to rent and return cars. It keeps track of available cars, customers, and active rentals. The project demonstrates **Object-Oriented Programming (OOP)** principles in Java, including encapsulation, inheritance, and polymorphism.  

### 🔹 Key Features  
✅ **Rent a Car** – Customers can rent an available car for a specified duration.  
✅ **Return a Car** – Customers can return a previously rented car.  
✅ **Manage Availability** – Cars are marked as unavailable when rented and become available upon return.  
✅ **Interactive Console Menu** – Users can navigate the system through a simple command-line interface.  

---

## ⚙️ Setup & Installation  

### **Prerequisites**  
Make sure you have the following installed:  
- **Java Development Kit (JDK 8 or later)**  
- **An IDE** (Eclipse, IntelliJ IDEA, or VS Code) or a text editor (Notepad++, Sublime, etc.)  
- **Command Prompt / Terminal** for running Java programs  

### **Steps to Set Up & Run**  

#### 🔹 **Clone or Download the Repository**  
If using Git:  
```bash
git clone https://github.com/your-username/car-rental-system.git
cd car-rental-system
```
Or **download** the project as a ZIP file and extract it.  

#### 🔹 **Compile the Java Files**  
Navigate to the project folder in the terminal:  
```bash
javac CarRentalSystem.java
```

#### 🔹 **Run the Application**  
```bash
java CarRentalSystem
```

#### 🔹 **Use the Interactive Menu**  
The system will display options:  
```
===== Car Rental System =====
1. Rent a Car
2. Return a Car
3. Exit
Enter your choice:  
```
Follow the instructions to rent or return cars.  

---

## 🛠️ Future Enhancements  
- ✅ **Database Integration** – Store car and customer details persistently.  
- ✅ **Graphical User Interface (GUI)** – Create a user-friendly desktop or web version.  
- ✅ **Pricing Models** – Add seasonal discounts or special offers.  

---

## 🤝 Contributing  
1. **Fork** the repository  
2. **Create a new branch** for changes  
3. **Commit & Push** your code  
4. **Open a Pull Request (PR)**  

---

🚀 **Happy Coding!** 🎯

This **Car Rental System** serves as a great starting point for learning **Object-Oriented Programming (OOP)** in Java! 🚗💨