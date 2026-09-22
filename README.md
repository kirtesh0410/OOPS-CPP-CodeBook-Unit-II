Brief description of Program :-

• **Public versus Private Inheritance :-**

This C++ program demonstrates the difference between **public inheritance and private inheritance**.

* The **`Base` class** contains a public function named `show()`.
* `PublicDerived` inherits from `Base` using **public inheritance**.
* The public `show()` function remains accessible through an object of `PublicDerived`.
* `PrivateDerived` inherits from `Base` using **private inheritance**.
* In private inheritance, the inherited public function becomes private within the derived class.
* The `callBaseShow()` function is provided to access `show()` from inside `PrivateDerived`.
* The program demonstrates how the **inheritance mode affects member accessibility**.

**In short:** The program demonstrates how **public and private inheritance change the accessibility of inherited base-class members**.
