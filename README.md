# OOPS-CPP-CodeBook-Unit-II
Object Oriented Programming with C++ - Unit II CodeBook

Student Name :- Kirtesh Bharambe

ZPRN :- 125UET1089

Class/Division :- SY AIDS C

Unit :- II

List of Programs :-

            1)Basic Single Inheritance  
            2)Protected Member Access  
            3)Public versus Private Inheritance  
            4)Multilevel Inheritance  
            5)Hierarchical Inheritance  
            6)Multiple Inheritance  
            7)Resolving Multiple-Inheritance Ambiguity  
            8)Constructor and Destructor Order  
            9)Parameterized Base Constructor  
            10)Function Overriding  
            11)Abstract Class  
            12)Virtual Base Class and Diamond Inheritance  
            13)Friend Class  
            14)Nested Class  
            15)Mini-Project :- Vehicle Rental System  
            16)Mini-Project :- Employee Payroll System  

Brief descriptions of each Program :-

• **1)Basic Single Inheritance :-**

This C++ program demonstrates **single inheritance** using `Person` as a base class and `Student` as a derived class.

* The **`Person` class** acts as the base class and stores the student's name.
* The **`Student` class** inherits from `Person` using public inheritance.
* The `Student` class contains its own data member, **`rollNumber`**.
* The derived class constructor initializes both the inherited name and its own roll number.
* The `displayStudent()` function displays the inherited name and student roll number.
* This demonstrates the **"is-a" relationship**, where a Student is a Person.

**In short:** The program demonstrates how a **derived class can inherit accessible members and functionality from a single base class**. 

• **2)Protected Member Access :-**

This C++ program demonstrates how a **derived class can access a protected member** of its base class.

* The **`Employee` class** contains a protected data member named `name`.
* The **`Developer` class** inherits from `Employee`.
* Since `name` is protected, it can be directly accessed inside the derived class.
* The `Developer` class also contains its own `language` data member.
* The `display()` function displays both the employee name and programming language.
* The program shows that protected members are accessible inside the base class and its derived classes.

**In short:** The program demonstrates the use of the **`protected` access specifier** for sharing data between a base class and its derived class. 

• **3)Public versus Private Inheritance :-**

This C++ program demonstrates the difference between **public inheritance and private inheritance**.

* The **`Base` class** contains a public function named `show()`.
* `PublicDerived` inherits from `Base` using **public inheritance**.
* The public `show()` function remains accessible through an object of `PublicDerived`.
* `PrivateDerived` inherits from `Base` using **private inheritance**.
* In private inheritance, the inherited public function becomes private within the derived class.
* The `callBaseShow()` function is provided to access `show()` from inside `PrivateDerived`.
* The program demonstrates how the **inheritance mode affects member accessibility**.

**In short:** The program demonstrates how **public and private inheritance change the accessibility of inherited base-class members**. 

• **4)Multilevel Inheritance :-**

This C++ program demonstrates **multilevel inheritance** using the hierarchy `Person → Employee → Manager`.

* The **`Person` class** is the base class and stores the person's name.
* The **`Employee` class** inherits from `Person` and adds an employee ID.
* The **`Manager` class** inherits from `Employee` and adds a team size.
* The `Manager` object can access functionality provided by both `Person` and `Employee`.
* The `showManager()` function displays the name, employee ID, and team size.
* This creates a three-level inheritance hierarchy.

**In short:** The program demonstrates how a class can inherit from another derived class to create a **multilevel inheritance structure**. 

• **5)Hierarchical Inheritance :-**

This C++ program demonstrates **hierarchical inheritance** using `Vehicle` as a common base class.

* The **`Vehicle` class** stores a vehicle registration number.
* The `Car` class inherits from `Vehicle` and provides an `openBoot()` function.
* The `Bike` class also inherits from `Vehicle` and provides a `helmetReminder()` function.
* Both derived classes can use the inherited `start()` function.
* The program creates separate objects for a car and a bike.
* This demonstrates a single base class having **multiple derived classes**.

**In short:** The program demonstrates **hierarchical inheritance**, where multiple classes inherit common functionality from one base class. 

• **6)Multiple Inheritance :-**

This C++ program demonstrates **multiple inheritance** using academic and sports records.

* The **`Academic` class** stores academic marks.
* The **`Sports` class** stores sports marks.
* The **`Student` class** inherits from both `Academic` and `Sports`.
* The student object can access functions from both base classes.
* The `showTotal()` function adds academic and sports marks.
* This demonstrates how one derived class can inherit from **two base classes**.

**In short:** The program demonstrates **multiple inheritance**, where a derived class inherits features from more than one base class. 

• **7)Resolving Multiple-Inheritance Ambiguity :-**

This C++ program demonstrates how to **resolve ambiguity in multiple inheritance** when two base classes contain functions with the same name.

* Both the **`Academic`** and **`Sports`** classes contain a function named `display()`.
* The `Student` class inherits from both classes.
* Calling `display()` directly through `Student` would create ambiguity.
* The **scope-resolution operator `::`** is used to specify which base-class function should be called.
* The `displayAll()` function explicitly calls both `Academic::display()` and `Sports::display()`.
* This allows the program to access both functions without ambiguity.

**In short:** The program demonstrates how the **scope-resolution operator** can be used to select the required function when multiple base classes contain members with the same name. 

• **8)Constructor and Destructor Order :-**

This C++ program demonstrates the **order in which constructors and destructors are executed** in inheritance.

* The `Base` class contains a constructor and destructor.
* The `Derived` class inherits from `Base` and also contains a constructor and destructor.
* When a derived object is created, the **base constructor executes first**.
* After the base constructor, the **derived constructor executes**.
* During object destruction, the **derived destructor executes first**.
* The base destructor executes after the derived destructor.
* This demonstrates the object lifecycle in an inheritance hierarchy.

**In short:** The program demonstrates that **construction occurs from Base to Derived, while destruction occurs from Derived to Base**. 

• **9)Parameterized Base Constructor :-**

This C++ program demonstrates how a **derived-class constructor initializes a parameterized base-class constructor**.

* The **`Person` class** contains a parameterized constructor that receives a person's name.
* The `Student` class inherits from `Person`.
* The `Student` constructor uses an **initializer list** to call the `Person` constructor.
* The student roll number is initialized in the derived class.
* The `display()` function displays the inherited name and roll number.
* This demonstrates how constructors can be connected across an inheritance hierarchy.

**In short:** The program demonstrates how a **derived constructor can pass values to and initialize a parameterized base constructor using an initializer list**. 

• **10)Function Overriding :-**

This C++ program demonstrates **function overriding** using virtual functions.

* The `Vehicle` class contains a virtual function named **`move()`**.
* The `Car` class overrides `move()` to display a road-related message.
* The `Boat` class also overrides `move()` to display a water-related message.
* The **`override` keyword** confirms that the derived function is intended to override the base function.
* The virtual function allows derived classes to provide their own implementation.
* This demonstrates **run-time polymorphic behavior**.

**In short:** The program demonstrates how a derived class can **override a virtual function** of its base class to provide specialized behavior. 

• **11)Abstract Class :-**

This C++ program demonstrates the use of an **abstract class and a pure virtual function**.

* The **`Shape` class** contains the pure virtual function `area()`.
* A pure virtual function is declared using **`= 0`**.
* Because `Shape` contains a pure virtual function, objects of `Shape` cannot be created directly.
* The `Rectangle` class inherits from `Shape` and implements the `area()` function.
* The `Circle` class also inherits from `Shape` and provides its own implementation of `area()`.
* Each derived class calculates its area according to its own formula.

**In short:** The program demonstrates how an **abstract base class with a pure virtual function** can define a common interface for derived classes. 

• **12)Virtual Base Class and Diamond Inheritance :-**

This C++ program demonstrates how a **virtual base class** is used to solve the diamond inheritance problem.

* The **`Person` class** acts as the common base class.
* Both `Student` and `Employee` inherit from `Person` using **virtual inheritance**.
* The `TeachingAssistant` class inherits from both `Student` and `Employee`.
* Virtual inheritance ensures that only **one `Person` part** exists in the final derived object.
* The `TeachingAssistant` constructor directly initializes the `Person` base.
* The program displays the name stored in the single shared `Person` part.

**In short:** The program demonstrates how a **virtual base class prevents duplicate copies of a common base class in diamond inheritance**. 

• **13)Friend Class :-**

This C++ program demonstrates how a **friend class** can access private data of another class.

* The `Account` class contains a private data member named `balance`.
* The `Auditor` class is declared as a **friend class** of `Account`.
* Because of friendship, `Auditor` can access the private `balance` member.
* The `inspect()` function of `Auditor` displays the account balance.
* The `Account` object is passed to the auditor for inspection.
* This demonstrates special access permission provided through a friend class.

**In short:** The program demonstrates how a **friend class can access private members of another class** when friendship is explicitly declared. 

• **14)Nested Class :-**

This C++ program demonstrates the creation and use of a **nested class**, which is a class defined inside another class.

* The outer class is named **`University`**.
* The `Department` class is defined inside the `University` class.
* The nested class stores the department name as a private data member.
* Its constructor initializes the department name.
* The `display()` function displays the department information.
* The nested class object is created using the scope-resolution syntax **`University::Department`**.

**In short:** The program demonstrates how a **class can be defined inside another class** and accessed using the outer class name. 

• **15)Mini-Project :- Vehicle Rental System :-**

This C++ program implements an **inheritance-based Vehicle Rental System** using a base `Vehicle` class and derived vehicle classes.

* The **`Vehicle` class** stores the registration number and rental rate per day.
* The `Car` class inherits from `Vehicle` and stores the number of doors.
* The `Bike` class inherits from `Vehicle` and stores the engine capacity.
* The `calculateRent()` function is used to calculate rental charges.
* The `Bike` class overrides `calculateRent()` and applies a **10% reduction** to the standard rental calculation.
* The `display()` function is overridden in the derived classes to display vehicle-specific information.
* The program demonstrates **inheritance, function overriding, and runtime polymorphism concepts** used in a practical application.
* The system calculates rental charges for three days for both a car and a bike.

**In short:** The program demonstrates how **inheritance and function overriding can be combined to build a simple vehicle rental application with different rental behavior for different vehicle types**. 

• **16)Mini-Project :- Employee Payroll System :-**

This C++ program implements an **Employee Payroll System** using an abstract base class and derived employee classes.

* The **`Employee` class** acts as an abstract base class.
* It stores common employee information such as **employee ID and name**.
* The pure virtual function **`calculateSalary()`** defines the salary calculation interface.
* The `PermanentEmployee` class calculates salary using **basic salary plus allowance**.
* The `ContractEmployee` class calculates salary using **hourly rate multiplied by hours worked**.
* The `displayPaySlip()` function accepts an `Employee` reference and displays employee details and calculated salary.
* Function overriding is used so that each employee type provides its own salary calculation.
* The program demonstrates **abstract classes, pure virtual functions, inheritance, function overriding, constructors, and polymorphism**.

**In short:** The program demonstrates how **inheritance and polymorphism can be used to create a flexible employee payroll system with different salary calculations for different employee types**. 

