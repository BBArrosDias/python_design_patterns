# Python Design Patterns

## Description

* This repository contains an overview of the Gang of Four (GoF) design patterns as outlined in their seminal book, together with modern-day variations, adjustments, discussions of intrinsic use of patterns in Python.

## Learning Objectives

* SOLID Design Principles:
  * [Single Responsibility Principle](/solid/single_responsibility.py)
  * [Open-Closed Principle](/solid/open_closed.py)
  * [Liskov Substitution Principle](/solid/liskov.py)
  * [Interface Segregation Principle](/solid/interface_segregation.py)
  * [Dependency Inversion Principle](/solid/dependency_inversion.py)
* Creational Design Patterns:
  * [Builder](/builder)
    * A builder is a separate component for building an object
    * Can either give builder an initializer or return it via a static function
    * To make builder fluent, return self
    * Different facets of an object can be built with different builders working in tandem via a base class
  * [Factories (Factory Method and Abstract Factory)](/factories)
    * A factory method is a static method that creates object
    * A factory is an entity that can take care of object creation
    * A factory can be external or reside inside the object as an inner class
    * Hierarchies of factories can be used to create related objects
  * [Prototype](/prototype)
    * To implement a prototype, partially construct an object and store it somewhere
    * Deep copy the prototype
    * Customize the resulting instance
    * A factory provides a convenient API for using prototypes
  * [Singleton](/singleton)
    * Different realizations of Singleton: custom allocator, decorator, metaclass
    * Laziness is easy, just init on first request
    * Monostate variation
    * Testability issues
* Structural Design Patterns:
  * [Adapter](/adapter)
    * Implementing an Adapter is easy
    * Determine the API you have and the API you need
    * Create a component which aggregates (has a reference to, ...) the adaptee
    * Intermediate representations can pile up: use caching and other optimizations
  * [Bridge](/bridge/bridge.py)
    * Decouple abstraction from implementation
    * Both can exist as hierarchies
    * A stronger form of encapsulation
  * [Composite](/composite)
    * Objects can use other objects via inheritance/composition
    * Some composed and singular objects need similar/identical behaviors
    * Composite design pattern lets us treat both types of objects uniformly
    * Python supports iteration with \_\_iter\_\_ and Iterable ABC
    * A single object can itself iterable by yielding self from \_\_iter\_\_
  * Decorator
  * Façade
  * Flyweight
  * Proxy
* Behavioral Design Patterns
  * Chain of Responsibility
  * Command
  * Interpreter
  * Iterator
  * Mediator
  * Memento
  * Observer
  * State
  * Strategy
  * Template
  * Method
  * Visitor

## Usage

* All files were created and compiled on Mac OS X 10.11 with Python3 (version 3.7)

## Awknowledgements

* Dmitri Nesteruk's course "Design Patterns in Python" on Udemy.com

---

## Author

* __Tu Vo__
