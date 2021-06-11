# High-Quality-Code
Design Patterns - Creational Patterns; Design Patterns - Structural Patterns; Design Patterns - Behavioral Patterns; Refactoring 
1. Creational Patterns:

    a) Singleton:
      - always is sealed class with: private static Singleton instance, private constructor and one getter- public static Singleton GetInstance (see Standard Singleton);
      - always is with only one instance;
      - Lazy and Eager loading in Singleton;       
      - real world usages: Logging, Managing a connection or a pool of connections to Database, Printer spooling, File, Configuration, Cache, Session based shopping cart;
    
    b) Simple Factory:
      - remember the drawing with the factory, which accept paper (like input) and produces paper boxes; the client doesn't know and doesn't understand factory logic;
      - creates objects without exposing the instantion logic to the client;
      - folder with enumeration;
      - static class Factory with method "CreateProduct"- accept the product type(enum) and return the whole product;
     
     c) Factory Method:
      - we create the object without exposing the creation logic. In this pattern, an interface is used for creating an object, but let subclass decide which class to instantiate. The           creation of object is done when it is required. The Factory method allows a class later instantiation to subclasses.
      
      d) Abstract Factory:      
      - remember this example: VW Factory creates doors for cars, windows for cars, tyres, but Honda Factory also creates doors for cars, windows for cars, tyres etc.
      - provides a way to encapsulate a group of individual factories that have a common theme without specifying their concrete classes;
      - every factory creates family of objects (doors, windows, tyres);
      
      e) Builder:
      - remember this example: BugattiChironBuilder (concrete builder for Buggati Chiron) with void SetModel(), void SetTransmission(), void SetBody(), void SetEngine;
      - multiply constructor in your class and might expand;
      - avoiding multiply parameters in constructors;
      
