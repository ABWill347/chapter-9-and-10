# chapter-9-and-10
Stack- Think of it as a temporary space where method calls and their local variables stay while the method runs. Once the method finishes, everything related to it is removed.

Heap -This is where objects live. When you create an object, it goes here. It's a more permanent space.

Object Creation- When you make a new object, you go through three steps: First, you declare a variable to hold it. Then, you create the object itself. Finally, you assign the object to the variable. Constructors are like blueprints for creating objects. They help set up the object's initial state.

The basic idea- Stack for short-term stuff, Heap for long-term storage of objects, and Constructors for setting up objects when they're created.
Let's simplify the main points:

Local Variables They exist only within the method they're declared in. Once the method ends, they vanish.

Instance Variables These live as long as the object they belong to. If the object is alive, so are its instance variables.

Scope vs. Life Scope refers to where you can use a variable (local variables within their method, instance variables within the object). Life refers to how long a variable persists (local variables until the method completes, instance variables until the object is gone).

Reference Variables Follow the same rules as primitives. An object is alive as long as there's a live reference to it. Once the last reference disappears, the object becomes eligible for garbage collection .

Garbage Collection- When an object is no longer reachable , GC cleans it up. Your job is to let go of objects when you're done so that GC can reclaim their memory.
.
Three Ways to Get Rid of an Object's Reference- The text outlines three methods for removing references to Java objects: when the reference goes out of scope, when it is assigned to another object, and when it is explicitly set to null.

Object Lifecycle-  the lifecycle of objects in Java, discussing the roles of instance variables and local variables. It highlights the differences in lifespan and behavior between these two types of variables.









Chapter 10

Math Methods
Purpose- Math methods in Java offer various operations beyond simple arithmetic, such as rounding, finding the minimum or maximum of two numbers, and obtaining the absolute value of a number.

Static Methods- Math methods are all static, meaning they don't require an instance of the Math class to be used.
Example- Math.round(42.2) rounds a floating-point number to the nearest integer, always returning the same result for the same input.

Difference Between Regular and Static Methods
Static Methods- These methods do not depend on instance variables and can be called without creating an instance of the class. They are typically utility methods.
Regular Methods- These methods typically rely on instance variables and require an instance of the class to be invoked.

Static Methods and Instance Variables
Incompatibility- Static methods cannot access instance variables because they are not associated with any particular instance of the class.
Error- Attempting to access an instance variable from a static method results in a compilation error because the static method doesn't know which instance's variable to use.

Static Variables
Shared Values- Static variables are shared among all instances of a class. They maintain a single value for the entire class.
Initialization- Static variables are initialized when the class is loaded. If not explicitly initialized, they receive default values .

Static Final Constants
Constant Variables- Marking a variable as static final makes it a constant, meaning its value cannot be changed once initialized.
Example- Math.PI is a static final constant representing the mathematical constant π.
Naming Convention- Constant variable names are typically written in all caps.

Benefits of Static Methods and Constants
Utility- Static methods and constants provide utility functions and values that can be accessed without creating instances of the class.



