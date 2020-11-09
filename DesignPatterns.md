
# Useful Links
https://www.tutorialspoint.com/design_pattern/design_pattern_interview_questions.htm

# What are design patterns?
Design patterns are documented tried and tested solutions for recurring problems in a given context. So basically you have a problem context and the proposed solution for the same. Design patterns existed in some or other form right from the inception stage of software development. Let’s say if you want to implement a sorting algorithm the first thing comes to mind is bubble sort. So the problem is sorting and solution is bubble sort. Same holds true for design patterns.

# Which are the three main categories of design patterns?
There are three basic classifications of patterns Creational, Structural, and Behavioral patterns. 

- Creational Patterns
    -  Abstract Factory:- Creates an instance of several families of classes
    - Builder: – Separates object construction from its representation
    -  Factory Method:- Creates an instance of several derived classes
    -  Prototype:- A fully initialized instance to be copied or cloned
    - Singleton:- A class in which only a single instance can exist
Note: – The best way to remember Creational pattern is by ABFPS (Abraham Became First President of States).

- Structural Patterns
    - Adapter:-Match interfaces of different classes.
    - Bridge:-Separates an object’s abstraction from its implementation.
    - Composite:-A tree structure of simple and composite objects.
    - Decorator:-Add responsibilities to objects dynamically.
    - Façade:-A single class that represents an entire subsystem.
    - Flyweight:-A fine-grained instance used for efficient sharing.
    - Proxy:-An object representing another object.
Note : To remember structural pattern best is (ABCDFFP)

- Behavioral Patterns
    - Mediator:-Defines simplified communication between classes.
    - Memento:-Capture and restore an object’s internal state.
    - Interpreter:- A way to include language elements in a program.
    - Iterator:-Sequentially access the elements of a collection.
    - Chain of Resp: – A way of passing a request between a chain of objects.
    - Command:-Encapsulate a command request as an object.
    - State:-Alter an object’s behavior when its state changes.
    - Strategy:-Encapsulates an algorithm inside a class.
    - Observer: – A way of notifying change to a number of classes.
    - Template Method:-Defer the exact steps of an algorithm to a subclass.
    - Visitor:-Defines a new operation to a class without change.
Note: – Just remember Music……. 2 MICS On TV (MMIICCSSOTV).

# What is Factory pattern?
Factory pattern is one of most used design pattern. This type of design pattern comes under creational pattern as this pattern provides one of the best ways to create an object.
In Factory pattern, we create object without exposing the creation logic to the client and refer to newly created object using a common interface.

# What is Abstract Factory pattern?
Abstract Factory patterns work around a super-factory which creates other factories. This factory is also called as factory of factories. This type of design pattern comes under creational pattern as this pattern provides one of the best ways to create an object.
In Abstract Factory pattern an interface is responsible for creating a factory of related objects without explicitly specifying their classes. Each generated factory can give the objects as per the Factory pattern.

# What is Singleton pattern, advantages and disadvantages?
- This pattern involves a single class which is responsible to create an object while making sure that only single object gets created. This class provides a way to access its only object which can be accessed directly without need to instantiate the object of the class.
- Singleton pattern is a creational pattern that restricts the instance of a class to just one single instance that will be able to coordinate actions across the whole system. The singleton design pattern is advantageous as it can be used over and over without the need to recreate a new object for every request. This is a huge time- and space-saver. However, the code becomes so tightly coupled that you can't make changes without affecting everything associated with it. It also doesn't support inheritance and can be easily broken.

# What are the difference between a static class and a singleton class?
Following are the differences between a static class and a singleton class.
- A static class can not be a top level class and can not implement interfaces where a singleton class can.
- All members of a static class are static but for a Singleton class it is not a requirement.
- A static class get initialized when it is loaded so it can not be lazily loaded where a singleton class can be lazily loaded.
- A static class object is stored in stack whereas singlton class object is stored in heap memory space.

# Differentiate factory and abstract factory design patterns.
You should be able to answer this question in one sentence. Being able to explain the difference concisely helps show your understanding of the design patterns.
Example: "The primary difference between them is as follows: a factory pattern is a method of creating a single object through inheritance, while an abstract factory pattern creates factory patterns, effectively producing families of related objects."