# Decorator Pattern — Coffee Ordering System

A Java implementation of the Decorator Design Pattern using a coffee ordering system.

The application allows customers to add milk, sugar, and whipped cream dynamically without modifying the original Espresso class.

## Project Structure

All Java source files are located in the root directory.

- Beverage.java — Component interface
- Espresso.java — Concrete Component
- BeverageDecorator.java — Abstract Decorator
- MilkDecorator.java — Adds $0.50
- SugarDecorator.java — Adds $0.20
- WhippedCreamDecorator.java — Adds $0.70
- Main.java — Main application
- README.md — Project documentation

## Requirements

- Java JDK 21 or compatible version
- Windows or another operating system supporting Java

## How to Run

Open Command Prompt in the project directory containing the Java files.

Compile the Java source files:


javac *.java


Run the application:

java Main



## Expected Output

```text
Espresso, Milk, Sugar, Whipped Cream
Cost: $3.40
```




## How It Works

1. Create an Espresso costing $2.00.
2. Add MilkDecorator (+$0.50).
3. Add SugarDecorator (+$0.20).
4. Add WhippedCreamDecorator (+$0.70).
5. Display the final description and total cost.

## Advantages

- Adds responsibilities dynamically at runtime.
- Avoids creating many subclasses.
- Supports the Open/Closed Principle.
- Promotes composition over inheritance.

## Possible Extension

A CaramelDecorator can be added to provide another optional ingredient without modifying existing classes.

## Conclusion

The Decorator Pattern provides a flexible solution for adding optional features to objects while keeping the original classes unchanged.
