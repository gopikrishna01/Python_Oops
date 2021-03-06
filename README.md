# Python Object Oriented Programming


### What is Oops:

 * Oops was invented in 1960
 * Oops is a paradigm(pattern) for code organization and design
 * Promotes collaboration, code extension and maintenance

### The Oops paradigm:
 * Organizes data into objects and functions into methods
 * Defines object specifications ( data and methods ) in classes

### Procedural Paradigm vs Object Paradigm:
* Procedural Paradigm

      def increment(val):
          return val+1

      this = 0
      this = increment(this)
      this = increment(this)
      print(this)

* Object Paradigm:

      class MyCustomInc(object):
          def __init__(self):
              self.val = 0
          def increment(self):
              self.val = self.val + 1
          def __repr__(self):
              return str(self.val)

      this = 0
      this = MyCustomInc()
      this.increment()
      print(this)

### Three pillers of Oops:

* Encapsulation
* Inheritance
* Polymorphism


### Modules Vs Classes

* Module is a file that containes python code
* Class  is a Python Code


#### Example:

      from collections import Counter

      #Here 
      #collections is a Module (Python file)
      #Counter is Class (Python Code)

### Some Definations:
##### 1. Class: Class is a blueprint for an Instance
##### 2. Instance: Instance is a constructed objcet of class
##### 3. Attribute: Attribute is object value: object.attribute
##### 4. Method: Method is a callable attribute defined in the class
##### 5. Object: Object is a unit of data (having one or more attributes) of a pirticular class or type with associated methods
##### 6. Self: self is the object on which the method was called

### Explanation of self:
When you call a metod in an Instance the instance get passed as the first argument.

#### Example for self explanation:
      class MyClass(object):
          def my_method(self):
              print(self)

      this = MyClass()
      this.my_method()
      print(this)
      
      """
      Code Out Put:
      <__main__.MyClass object at 0x7ff7482b3b70>
      <__main__.MyClass object at 0x7ff7482b3b70>
      """
      
##### NOTE: In the above code if we observe self hex code and this object hex code are same which tells us that instance get passed as the first argument to the method.
