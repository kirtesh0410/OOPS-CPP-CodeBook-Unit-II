Brief descriptions of each Program :-

• **Resolving Multiple-Inheritance Ambiguity :-**

This C++ program demonstrates how to **resolve ambiguity in multiple inheritance** when two base classes contain functions with the same name.

* Both the **`Academic`** and **`Sports`** classes contain a function named `display()`.
* The `Student` class inherits from both classes.
* Calling `display()` directly through `Student` would create ambiguity.
* The **scope-resolution operator `::`** is used to specify which base-class function should be called.
* The `displayAll()` function explicitly calls both `Academic::display()` and `Sports::display()`.
* This allows the program to access both functions without ambiguity.

**In short:** The program demonstrates how the **scope-resolution operator** can be used to select the required function when multiple base classes contain members with the same name.
