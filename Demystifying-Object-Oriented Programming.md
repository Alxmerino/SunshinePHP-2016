# Demystifying Object-Oriented Programming

### Alena Holligan | @sketchings | [www.sketchings.com](http://www.sketchings.com)

* * *


## What is OOP?

* A programming concept that treats functions and data as objects

* A programming methodology based on objects, instead of functions and procedures

## Notes

* Variables inside of a class is called a property

* All functions inside of a class are called methods

## Class

A template/blueprint that facilitates creation of objects. A set of functions and variables as methods and properties

## Object 

an Instance of a class

## Abstraction

An abstraction denotes the essential characteristics of an object that distinguish it from all other kinds of objects.

## Encapsulation

* Scope. Controls who can access what. Restrict to some of the object's components (properties and methods), preventing unauthorized access.

* Public - everyone

* Protected - inherited classes

* Private - class itself, no children

## Constructor Method & Magic Methods

* __construct()..

* __toString

* [http://php.net/manual/en/language.oop5.magic.php](http://php.net/manual/en/language.oop5.magic.php)

## Inheritance: Passes knowledge down

* Subclass: parent and child relationship, allows for reusability and extensibility

* Additional code to an existing class

* NUTSHELL: create a new class based on an existing class with more data, create new objects based on this class.

## Polymorphism

Polymorphism describes a pattern in OOP in which classes have different functionality while sharing a common interface

## Interface

* Interface, specifies which methods a class must implement

* All methods in an interface must be public

* Multiple interfaces can be implemented by using comma separation

* Interface may contain a CONSTANT, but may not be overridden by implementing class
`interface UserInterface { … }
class User implements UserInterface { … }

## Abstract

An abstract class is a mix between an interface and a class. It can define functionality as well as interface (in the form of abstract methods). Classes extending an abstract class must implement all of the abstract methods defined in the abstract class.

## Namespaces

* Help create a new layer of code encapsulation

* Keep properties from colliding between areas of your code

* Only classes, interfaces, functions and constants are affected

* Anything that does not have a namespace is considered in the Global namespace (namespace = "")

* must be declared first (except 'declare)

* Can define multiple in the same file

* You can define that something be used in the "Global" namespace by enclosing a non-labeled namespace in {} brackets.

* Use namespaces from within other namespaces, along with aliasing

