Brief description of Program :-

• **Constructor and Destructor Order :-**

This C++ program demonstrates the **order in which constructors and destructors are executed** in inheritance.

* The `Base` class contains a constructor and destructor.
* The `Derived` class inherits from `Base` and also contains a constructor and destructor.
* When a derived object is created, the **base constructor executes first**.
* After the base constructor, the **derived constructor executes**.
* During object destruction, the **derived destructor executes first**.
* The base destructor executes after the derived destructor.
* This demonstrates the object lifecycle in an inheritance hierarchy.

**In short:** The program demonstrates that **construction occurs from Base to Derived, while destruction occurs from Derived to Base**.
