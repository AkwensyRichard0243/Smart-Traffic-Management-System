# POLYMORPHISM-Traffic-Management-System

## Overview
This project demonstrates the concept of **Polymorphism** in Object-Oriented Programming (OOP) using Python. It models a Smart Traffic Management System where different traffic devices respond to the same `activate()` command in different ways.

The project also showcases other OOP principles such as **Inheritance**, **Encapsulation**, and **Method Overriding**.

---

## Features
- Parent class: `TrafficDevice`
- Child classes:
  - `TrafficLight`
  - `SpeedCamera`
  - `PedestrianSignal`
  - `EmergencySiren`
- Uses **polymorphism** to activate all devices through a single loop.
- Demonstrates **encapsulation** using private attributes and getter methods.
- Demonstrates **inheritance** and **method overriding**.

---

## Project Structure

```
POLYMORPHISM-Traffic-Management-System/
│
├── traffic_management.py
└── README.md
```

---

## How It Works

Each traffic device inherits from the `TrafficDevice` class and overrides the `activate()` method to perform its own unique task.

Instead of checking the type of each object, all devices are stored in a list and activated using a single loop.

Example:

```python
for device in devices:
    device.activate()
```

This demonstrates **runtime polymorphism**, where the correct `activate()` method is called based on the object's class.

---

## Sample Output

```text
Smart Traffic Management System

Traffic Light: Changing lights (Red → Yellow → Green).
Speed Camera: Capturing speeding vehicles.
Pedestrian Signal: Displaying WALK signal for pedestrians.
Emergency Siren: Sounding emergency alert for priority vehicles.
```

---

## OOP Concepts Demonstrated

### Encapsulation
- The device name is stored as a private attribute.
- A getter method is used to access the value.

### Inheritance
- All traffic devices inherit from the `TrafficDevice` parent class.

### Method Overriding
- Each child class provides its own implementation of the `activate()` method.

### Polymorphism
- The same `activate()` method call produces different behaviors depending on the object.

---

## Requirements

- Python 3.x

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/POLYMORPHISM-Traffic-Management-System.git
```

2. Navigate into the project folder:

```bash
cd POLYMORPHISM-Traffic-Management-System
```

3. Run the program:

```bash
python traffic_management.py
```

---
 Author

Akwensy Richard

---



