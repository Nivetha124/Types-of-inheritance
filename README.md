# Types-of-inheritance

# SINGLE INHERITANCE 
parent(base class), child (derived class) { derived class inherit from the base class}
# Real time example
    *  Dog class inherits the Animal class
    *  Student class inherits the College class
    *  Car class inherits the Vehicle class
eg:  class Animal:
        def Walking(self):
            print("animal") 
     class Dog(Animal):
        def Eating(self):
            print("dog") 
     obj=Dog()
     obj.Eating()
     obj.Walking()

# MULTI-LEVEL INHERITANCE
grandparent(base) , parent(intermediate), child(derived) 
# Real time example
  *  a child inheriting from his father who inherited from his grandfather
  *  staff inherits from Hod who inherits from principle
    eg: Class Grandfather:
           def gdisplay(self):
               print("grandfather")
        class Parent(Grandfather):
           def pdisplay(self):
               print("parent")
        class Son(Parent):
           def sdisplay(self):
               print("son")
        obj=Son()
        obj.sdisplay()
        obj.pdisplay()
        obj.gdisplay()
     
# HIERARICAL INHERITANCE
  A parent have two child or more.{one base class have multiple derived class}
# Real Time example:
    * we created a parent class(base class) called VEHICLE and two subclasses TWOWHEELER and FOURWHEELER which extends the base class Vehicle. Hence apart from accessing their own methods and properties, these classes can also access the methods and properties of the "Vehicle" class.
    * HOUSE is a base class and 2BHK,3BHK,4BHK are the derived class.
    * ECE Department is a base class and A,B,C section are the derived class.
    eg: class ECE:
           def edisplay(self):
               print("ece")
         class Asection(ECE):
           def display(self):
               print("A section in ece dept")
         class Bsection(ECE):
           def bdisplay(self):
               print("B section in ece dept")
         obj=Asection()
         obj.display()
         obj.edisplay()
         obj1=Bsection()
         obj.bdisplay()
         obj.edisplay()

# MULTIPLE INHERITANCE
  two base class both have one Or more derived class
  # Real time example:
     * A class that inherits from both a "VEHICLE" class and an "ELECTRICITY-POWERED" class, to create a new class called "ELECTRIC VEHICLE". This class would have access to both the properties and methods of its parent classes.
     * OWNER class and HOUSE class to create a new class called RENTAL.
     * CAR class and BUS class to create a new class called VEHICLE.
     eg:
     class Father:
        def display(slef):
            print("father")
    class Mother:
       def mdisplay(self):
           print("mother")
    class son(Father,Mother):
       def sdisplay(self):
           print("son")
  
