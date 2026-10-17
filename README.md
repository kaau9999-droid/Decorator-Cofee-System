# Decorator Pattern — Coffee Ordering System

A Java implementation of the Decorator design pattern, based on the coffee
ordering example: a base `Espresso` is wrapped in `MilkDecorator`,
`SugarDecorator`, and `WhippedCreamDecorator` to build up description and
price dynamically at runtime.

## Structure

```
DecoratorPatternDemo/
├── src/
│   ├── Beverage.java              # Component interface
│   ├── Espresso.java              # Concrete Component
│   ├── BeverageDecorator.java     # Abstract Decorator
│   ├── MilkDecorator.java         # Concrete Decorator (+$0.50)
│   ├── SugarDecorator.java        # Concrete Decorator (+$0.20)
│   ├── WhippedCreamDecorator.java # Concrete Decorator (+$0.70)
│   └── Main.java                  # Client code / entry point
└── README.md
```

## Run it in VS Code

1. Open this folder in VS Code (`File > Open Folder...`).
2. Install the **Extension Pack for Java** (Microsoft) if you don't have it —
   VS Code will usually prompt you automatically.
3. Open `src/Main.java` and click **Run** above the `main` method
   (or press `F5`).

## Run it from the terminal

Requires a JDK (11+) on your PATH.

```bash
cd DecoratorPatternDemo
javac -d bin src/*.java
java -cp bin Main
```

## Expected output

```
Espresso, Milk, Sugar, Whipped Cream
Cost: $3.4
```

## Try extending it

Add a `CaramelDecorator` following the same shape as `MilkDecorator`
(+$0.60, appends ", Caramel") without touching any existing class —
that's the Open/Closed Principle in action.
