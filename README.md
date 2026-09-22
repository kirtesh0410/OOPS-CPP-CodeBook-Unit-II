Brief description of Program :-

• **Friend Class :-**

This C++ program demonstrates how a **friend class** can access private data of another class.

* The `Account` class contains a private data member named `balance`.
* The `Auditor` class is declared as a **friend class** of `Account`.
* Because of friendship, `Auditor` can access the private `balance` member.
* The `inspect()` function of `Auditor` displays the account balance.
* The `Account` object is passed to the auditor for inspection.
* This demonstrates special access permission provided through a friend class.

**In short:** The program demonstrates how a **friend class can access private members of another class** when friendship is explicitly declared.
