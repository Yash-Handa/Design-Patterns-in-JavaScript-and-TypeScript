# Builder Design Pattern :construction_worker:

Builder pattern aims to “Separate the construction of a complex object from its representation so that the same construction process can create different representations.” It is used to construct a complex object step by step and the final step will return the object. The process of constructing an object should be generic so that it can be used to create different representations of the same object.

Builder Pattern is used mostly when large number of deferent types of objects are to be made but these objects use same object building processes (i.e., objects have same methods but those methods do a bit different stuff)

## Explanation with Example

In this example there is a CIVILEngineer class that creates many different types of houses (objects) based on the object of the house blueprint classes. This example contains:

1. **House class:** This class has methods for creating different parts of the house: setRoof(), setFloor(), setInterior(), setWalls(), etc
2. **house blueprint classes:** Many other classes like **IglooBlueprint class**, **TentHouseBlueprint class**, **BambooHutBlueprint class**, etc creates an object of the **House class** and calls its methods with specific parameters to modify the object creation. Eg: **IglooBlueprint class** has a method `buildWalls()` which calls `house.setWalls('Ice blocks')`.
3. **CIVILEngineer class:** This class takes an object of one of the **house blueprint classes** and returns an object of **House class**

<div>
  <img alt="Builder Pattern Example" title="Builder Pattern Example" src="/Creational Design Patterns/Builder/Builder Design Pattern Example.png">
</div>
