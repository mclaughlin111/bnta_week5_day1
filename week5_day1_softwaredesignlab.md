### 1. What do we mean by **coupling** and **cohesion** when discussing structured design?

In stuctured design the main problem is broken down into several smaller 	problems: this is known as the 'divide and conquer' strategy'.
	
The smaller sections of the problem are solved by use of "solution modules"; 	these modules are arranged in hierarchy and communicate with each other. 
	
Two rules for good Structure design are: 
	
**Cohesion** - the grouping of all functionally related elements
	
**Coupling** - communication between different modules
	
Good structured design has high cohesion and low coupling arrangments. 

### 2. What is the difference between **top-down** and **bottom-up** design? Which best describes a function oriented design?

In Top-down design, you seek to break the problem into smaller parts whereas in a bottom-up design you solve smaller problems/(modules) and integrate it as whole to complete the solution. 

Function Oriented Design could be seen as a predominantly top-down approach as this model breaks problems down into a series of interacting pieces or modules, each with a distinct function. 

### 3. In which design methodology would a **class diagram** be most useful?

Object Oriented Design (as it relies on a system  of classes and objects that employ methods and have attributes)
 
### 4. What are the four pillars of object oriented programming? Give a single-sentence description of each.

1. Abstraction: *The property within Object Oriented proggraming which allows objects to inherit by extending classes and implement methods via interfaces.* E.g. `Audi` extends abstract Class `Car`, Implements interface `IMachine`


1. Encapsulation: *The feature of an object that makes it's methods & attributes private (removing access to parts of your code and giving each object control over it's state* eg. `Private String Name`;


1. Inheritance: *A 'concrete' class will inherit any and all attributes of it's parent class which it extends.* Eg. `Public Class Orchestra Extends Ensemble`


1. Polymorphism: *In object oriented proggraming the ability to create a property, function, or object that has more than one realization. Polymorphism is the ability to substitue classes that have common functionality in sense of methods and data.* E.g. An `IDrive` interface would allow you to drive any car regardless of make or model

### 5. What is the strategy pattern? How would its implementation differ between a functional and object oriented system?

In Strategy pattern, a class or object can be changed at run time. You create objects which represent various strategies and a context object whose behaviour varies as per its strategy object. The strategy object changes the executing algorithm of the context object. 

The motivation for use of strategy pattern is in situations when classes differ only in their behavior. For this cases is a good idea to isolate the algorithms in separate classes in order to have the ability to select different algorithms at runtime. You intend to define a family of algorithms, encapsulate each one, and make them interchangeable. Strategy lets the algorithm vary independently from clients that use it.

In strategy pattern, methods/classes/algorithms are subject to change at runtime. It is built around a system of functions as opposed to modelling real-systems with objects and classes. 

### 6. Imagine you are creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

**Object Oriented Design:** with a potential leaning toward a top-down planning stage. 

This would allow a system that can be adapted and manipulated toward the 'lower level' classes and allow for granularity and customisabiltiy in the form of polymorphism and interfaces. 

E.g. any payment vendor could use an interface `IPay` but the fine details of each transaction can be tailored to the specific use case/class.



