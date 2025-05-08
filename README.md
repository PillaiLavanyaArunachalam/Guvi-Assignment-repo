Solutions

Answer 1: C. There is no default constructor defined.

Answer 2: C. Compilation error

Answer 3: B. 20 — obj2 and obj1 refer to the same object

Answer 4: C. NullPointerException

Answer 5: The output is "null" because of the way Java handles constructors in inheritance. When we create a Dog object, the constructor of the parent class Animal runs first. Inside this constructor, the overridden speak() method is called, but the Dog constructor hasn't had a chance to initialize the sound variable yet. In Java, instance variables like sound default to null if not explicitly set, so the method tries to print sound.toUpperCase() on a null value, which results in "null" being printed instead of the expected "BARK".
