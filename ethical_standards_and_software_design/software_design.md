# Software Design

## What do we mean by coupling and cohesion when discussing structured design?

Coupling refers to the degree of interdependence between modules. It essentially measures how tightly connected different parts of your code are. Low coupling is the most ideal. This means modules should be as independent as possible, with minimal reliance on each other's internal workings. Changes in one module should have minimal impact on others in theory.

On the other hand, cohesion refers to how focused and related the elements within a single module are. It describes how well the functions and data structures within a module work together towards a single purpose. In simpler terms, it's about how "stuck together" the things inside a module are. A module with high cohesion has elements that all contribute to a single, well-defined task.

## What is the difference between top-down and bottom-up design? Which best describes a function oriented design?

Top-down design starts with a high-level overview of the entire system, focusing on the big picture and overall functionality. This big picture is then broken down progressively into smaller, more manageable components and sub-functions. On the other hand, bottom-up design begins with the development of individual building blocks or low-level modules with specific functionalities. These independent modules are then integrated and assembled to create a more complex system.

Top-down design best a function oriented approach. This is because of several reasons:
1) Function-oriented design emphasizes breaking down the problem into smaller, well-defined functions with clear purposes.
2) This aligns with the top-down philosophy of starting with the overall functionality and then decomposing it into manageable units.
3) In function-oriented design, these functions become the building blocks you use to create the entire system.

## In which design methodology would a class diagram be most useful?

The class diagram would be most useful in Object-Oriented Design. This is because of several reasons:

1) Object-Oriented Design allows to plan and visualize the structure of their object-oriented system.
2) Improve communication and collaboration within the development team.
3) Identify potential design issues early on in the development process.
4) Document the system for future reference and maintenance.

## What are the four pillars of object oriented programming?

1) Abstraction: Focusing on the essential details while hiding unnecessary complexity.
2) Encapsulation: Bundling data and methods together within a single unit (class) for data protection and controlled access.
3) Inheritance: Creating new classes (subclasses) that inherit properties and behaviors from existing ones (superclasses) for code reusability.
4) Polymorphism: Allowing objects of different classes to respond differently to the same message, promoting flexible and dynamic behavior.

## What is the strategy pattern? How would its implementation differ between a functional and object oriented system?

The strategy pattern is a behavioral design pattern that lets you dynamically select an algorithm at runtime. It does this by: defining a family of algorithms as separate classes or functions, having a central context object and allowing the context object to switch between different strategies. 

Within a Functional approach, strategies are implemented as separate functions and the context object passes data to the chosen strategy function to perform the specific operation whereas within an Object Oriented Approach, strategies are implemented as separate classes that inherit from a common interface and 
the context object holds a reference to a strategy object and delegates the work to its methods.

## Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

I would suggest following the Object Oriented Design (OOD) methodology due to several reasons:

1) Flexibility and Reusability: OOD promotes creating reusable components (classes) that encapsulate data (payment methods, user details) and functionality (processing transactions, handling refunds). This is crucial for a system that needs to handle diverse payment scenarios across various sectors.

2) Modularity and Maintainability: With OOD, you can break down the payment system into smaller, well-defined classes like PaymentProcessor, Order, and User. This modularity makes the system easier to understand, maintain, and modify as new features or integrations become necessary.

3) Scalability:  An object-oriented approach allows you to easily add new functionalities or payment methods by extending existing classes or creating new ones. This is essential for a payment system aiming for wide adoption and future growth.

4) Real-World Representation: OOD maps well to real-world entities involved in online payments (users, orders, payment processors). This makes the code more intuitive for developers to understand and reason about.

Even though other methodologies have their advantages, structured design offers strong organization but may lack the flexibility needed for a multifaceted system and function-oriented design can create well-defined functions but might struggle with complex interactions between functionalities. However, OOD provides a strong foundation for building a robust, adaptable, and maintainable online payment system that can cater to various sectors and payment scenarios.





