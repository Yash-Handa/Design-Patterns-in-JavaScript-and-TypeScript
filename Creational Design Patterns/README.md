# Creational Design Patterns :baby:

Creational design patterns are design patterns that deal with **object creation mechanisms**, trying to create objects in a manner suitable to the situation. The basic form of object creation could result in design problems or added complexity to the design. Creational design patterns solve this problem by somehow controlling this object creation.

In other words, Creational design patterns are used when a decision must be made at the time of instantiation of a class (i.e. creating an object of a class). These patterns makes dynamic (on run time) object creation easier.  
Traditionally, objects are made from classes by hard coding them with the `new` operator but these Design Patterns abstracts this step and the end users don't have to manually create an object.

**Traditional Method:**

```js
const userJohn = new User('John');
```

In both JavaScript and TypeScript `new` keyword is used for object creation from the class

- *userJohn*: The created object is stored in the variable called userJohn.
- *User*: User is the name of the class whose object is created by the `new` operator (the actual class creation is not shown in the example).

## Types of Creational Design Patterns

There are 5 Creational Design Patterns. Each pattern creates objects from classes in a particular way – in particular contexts.

| **DESIGN PATTERN**    | **Description / Purpose** |
|:---------------------:|:-------------------------:|
|[**Builder**](/Builder/README.md)            |Builder design pattern is a way to construct complex objects and should be used only when we want to build different types of immutable objects using same object building process.|
|[**Prototype**](/Prototype/README.md)          |Prototype design pattern is used in scenarios where application needs to create a large number of instances of a class, which have almost same state or differ very little.|
|[**Factory**](/Factory/README.md)            |Factory design pattern is most suitable when complex object creation steps are involved. To ensure that these steps are centralized and not exposed to composing classes.|
|<a href="/Abstract Factory/README.md">**Abstract Factory**</a>   |Abstract Factory pattern is used whenever we need another level of abstraction over a group of factories created using factory pattern.|
|[**Singleton**](/Singleton/README.md)          |Singleton pattern is used to ensure a class has only one instance and provide a global point of access to it.|

<hr>
<div>
  <p><i><a href="../README.md"><b><-- Home</b></a></i></p>
  <p align="right"><i>Next: <a href="/Builder/README.md"><b>Builder Design Pattern --></b></a></i></p>
</div>
