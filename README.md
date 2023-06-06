# OOPS


# Object :

Any entity that has state and behavior is known as an object. For example, a chair, pen, table, keyboard, bike, etc. It can be physical or logical.

An Object can be defined as an instance of a class. An object contains an address and takes up some space in memory. Objects can communicate without knowing the details of each other’s data or code. The only necessary thing is the type of message accepted and the type of response returned by the objects.

Example: A dog is an object because it has states like color, name, breed, etc. as well as behaviors like wagging the tail, barking, eating, etc.

# Class :

Collection of objects is called class. It is a logical entity.

A class can also be defined as a blueprint from which you can create an individual object. Class doesn’t consume any space.

# Inheritance :
When one object acquires all the properties and behaviors of a parent object, it is known as inheritance.

![image](https://github.com/sree-hari55/OOPS/assets/59191028/ab5c5148-884e-46b2-ac63-a534fc63182f)

# Encapsulation :
Encapsulation is a mechanism where you bind your data and code together as a single unit. It also means to hide your data in order to make it safe from any modification. What does this mean? The best way to understand encapsulation is to look at the example of a medical capsule, where the drug is always safe inside the capsule. Similarly, through encapsulation, the methods and variables of a class are well hidden and safe.

# Polymorphism
Polymorphism means taking many forms, where ‘poly’ means many and ‘morph’ means forms. It is the ability of a variable, function or object to take on multiple forms. In other words, polymorphism allows you define one interface or method and have multiple implementations.

# Types of Polymorphism in Java :
 
 1) Runtime polymorphism
 2) Compile time polymorphism
 
# Runtime Polymorphism:
In Java, runtime polymorphism refers to a process in which a call to an overridden method is resolved at runtime rather than at compile-time. In this, a reference variable is used to call an overridden method of a superclass at runtime. Method overriding is an example of runtime polymorphism. Let us look the following code to understand how the method overriding works:

public Class BowlerClass{
void bowlingMethod()
{
System.out.println(" bowler ");
}
public Class FastPacer{
void bowlingMethod()
{
System.out.println(" fast bowler ");
}
Public static void main(String[] args)
{
FastPacer obj= new FastPacer();
obj.bowlingMethod();
}
}
# Compile Time Polymorphism:

In Java, compile-time polymorphism refers to a process in which a call to an overloaded method is resolved at compile time rather than at runtime. Method overloading is an example of compile time polymorphism. Method Overloading is a feature that allows a class to have two or more methods having the same name but the arguments passed to the methods are different.

Unlike method overriding, arguments can differ in:

Number of parameters passed to a method
Datatype of parameters
The sequence of datatypes when passed to a method.


# Association
Association is a relation between two separate classes that establish through their Objects. Association can be one-to-one, one-to-many, many-to-one, many-to-many.
In Object-Oriented programming, an Object communicates to other Objects to use functionality and services provided by that object.
There are two forms of association

Composition
Aggregation

# Composition :

Composition is an association that represents a part of a whole relationship where a part cannot exist without a whole. If a whole is deleted then all parts are deleted. It has a stronger relationship.

# Key Points :

It represents a part-of-relationship.
In composition, both entities are dependent on each other.
When there is a composition between two entities, the composed object cannot exist without the other entity. For example, if order HAS-A line-items, then an order is a whole, and line items are parts. If an order is deleted then all corresponding line items for that order should be deleted.
Favor Composition over Inheritance.
# Implementation with Example :
Let's take the example of Placing an Order. If order HAS-A line-items, then an order is a whole, and line items are parts. If an order is deleted then all corresponding line items for that order should be deleted.

# Aggregation :

Aggregation is an association that represents a part of a whole relationship where a part can exist without a whole. It has a weaker relationship.
It is a specialized form of Association where all object has their own lifecycle but there is ownership. This represents a “whole-part or a-part-of” relationship.
Let’s take an example of the relationship between the Department and the Teacher. A Teacher may belong to multiple departments. Hence Teacher is a part of multiple departments. But if we delete a Department, the Teacher Object will not destroy.


# Key Points :
It represents the Has-A relationship.
It is a unidirectional association i.e. a one-way relationship. For example, the department can have students but vice versa is not possible and thus unidirectional in nature.
In Aggregation, both the entries can survive individually which means ending one entity will not affect the other entity.

# Coupling 
Coupling refers to the degree to which one class knows about another class. If one class uses another class, that is coupling. Low dependencies between “artifacts” (classes, modules, components).There shouldn’t be too much of dependency between the modules, even if there is a dependency it should be via the interfaces and should be minimal.

While creating a complex application in java, the logic of one class will call the logic of another class to provide the same service to the clients.
If one class calling another class logic then it is called collaboration.
When one class is collaborating with another class then there exists tight-coupling between the two classes.
If one class wants to call the logic of a second class then they first-class need an object of second class it means the first class creates an object of second class.

# cohesion :
The term cohesion is used to indicate the degree to which a class has a single, well-focused responsibility. Cohesion is a measure of how the methods of a class or a module are meaningfully and strongly related and how focused they are in providing a well-defined purpose to the system.
Refernces :
https://medium.com/edureka/object-oriented-programming-b29cfd50eca0
https://rameshfadatare.medium.com/oops-concepts-in-java-eb2ad6f53b69
