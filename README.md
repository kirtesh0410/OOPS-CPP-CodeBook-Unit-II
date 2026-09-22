Brief description of Program :-
 
• **Virtual Base Class and Diamond Inheritance :-**

This C++ program demonstrates how a **virtual base class** is used to solve the diamond inheritance problem.

* The **`Person` class** acts as the common base class.
* Both `Student` and `Employee` inherit from `Person` using **virtual inheritance**.
* The `TeachingAssistant` class inherits from both `Student` and `Employee`.
* Virtual inheritance ensures that only **one `Person` part** exists in the final derived object.
* The `TeachingAssistant` constructor directly initializes the `Person` base.
* The program displays the name stored in the single shared `Person` part.

**In short:** The program demonstrates how a **virtual base class prevents duplicate copies of a common base class in diamond inheritance**.
