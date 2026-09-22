Brief description of Program :-


• **Abstract Class :-**

This C++ program demonstrates the use of an **abstract class and a pure virtual function**.

* The **`Shape` class** contains the pure virtual function `area()`.
* A pure virtual function is declared using **`= 0`**.
* Because `Shape` contains a pure virtual function, objects of `Shape` cannot be created directly.
* The `Rectangle` class inherits from `Shape` and implements the `area()` function.
* The `Circle` class also inherits from `Shape` and provides its own implementation of `area()`.
* Each derived class calculates its area according to its own formula.

**In short:** The program demonstrates how an **abstract base class with a pure virtual function** can define a common interface for derived classes.
